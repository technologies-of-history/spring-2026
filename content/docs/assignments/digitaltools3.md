---
layout: page
bookTOC: false
draft: false
title: Digital Tools 3
---
# Turning texts into data with XML and EditionCrafter
As you know from class, XML is a metalanguage (a language used to describe or markup another language) used in order to process and store texts in digital format. Markup languages are valuable as means of helping digital archivists and instructional technologists do two things: first, markup creates a rich data set from the text in question which can then be converted into a number of formats; second, markup encodes how a particular text should be presented on a webpage, digital publication, data set, etc. Markup languages thus guide our interpretations of those texts. Considerations like spacing, bolding, and headings are all aspects of the markup process—which is often also referred to as “encoding.” Marking up a document in XML is a matter of directing a person as to how the manuscript’s content should be presented and interpreted.

For this assignment, you will select a Middle English medical recipe from [Trinity College Cambridge MS O.8.35](https://mss-cat.trin.cam.ac.uk/Manuscript/O.8.35) in order to create your own TEI markup.

## Trinity College Cambridge MS O.8.35, digitized by the Trinity College Cambridge Library

{{< iframe url="https://projectmirador.org/embed/?iiif-content=https://mss-cat.trin.cam.ac.uk/Manuscript/O.8.35/manifest.json" >}}


## Step 1: Transcribe a page of text

1. Click through the images of TCC MS O.8.35 and select a single page of text to transcribe. Make note of the folio number for your page, indicated at the bottom of the Mirador viewer (i.e. f001r or f014v).
2. Once you've located the folio number, visit our GitHub course site and navigate to dyngley_data > dyngley.xml.
3. Scroll through the XML code under `<facsimile sameAs="https://mss-cat.trin.cam.ac.uk/Manuscript/O.8.35/manifest.json">` until you find your folio number. 
Each image of the manuscript has been given an xml id, which then corresponds to a folio number. For example, in this line of code 
```<surface xml:id="f016" ulx="0" uly="0" lrx="2967" lry="4062" sameAs="https://mss-cat.trin.cam.ac.uk:8183/iiif/2/O.8.35%2F017_O.8.35_f001r.jp2" ><label>f001r</label><graphic mimeType="application/json" url="https://mss-cat.trin.cam.ac.uk:8183/iiif/2/O.8.35%2F017_O.8.35_f001r.jp2"/></surface>```
the xml id is "f016" while the actual folio number of the manuscript is "f001r."
That's because this is the sixteenth image in the manuscript, though it corresponds with the first official numbered folio of the manuscript.
4. Create a .txt file using your text editor. Use the following naming convention: the_xml_id_for_your_page.txt. For example, the file featuring the transcriptions of f001r of the manuscript would be named f016.txt.
5. Transcribe the entire recipe in your text file.
6. Upload your .txt file to our GitHub course site in the folder dyngley_data > transcriptions, following our GitHub submission protocols. Create a branch named **yourlastname_transcription**. Upload the file to the **transcriptions** folder within **dyngley_data***. Finish by submitting a pull request to the **master** branch of our repository. 

Once I've looked over your transcription, I'll merge your file into the larger XML file for the critical edition. Your work will appear on the


## Step 2: Mark-up your transcription using TEI in Markdown

1. In your text editor, create an .md file to compose your blog post with TEI mark-up. 
2. Somewhere in that .md file, copy your transcription text from your .txt file. 
3. Encode the body of the text. Your TEI encoding should follow standard format, incorporating `<title>`, `<PersonName>`, and `<measure>` and other tags within the TEI glossary as necessary. You can refer to the glossary of official TEI elements [here](https://tei-c.org/release/doc/tei-p5-doc/en/html/REF-ELEMENTS.html), or you can review the basic TEI tags in the [Basic Tagging tutorial](https://www.wwp.northeastern.edu/outreach/seminars/_current/presentations/basic_encoding/basic_encoding_tutorial_00.xhtml) from the Women Writer's Project. (Remember that you'll want your mark-up to show up as code on our website, which means you'll need to use the appropriate Markdown syntax to set off your code from the rest of your blog post. (Hint: bracket your markup code with triple ticks at the start and at the end. You can always refer back to the [Getting Started with Markdown](https://programminghistorian.org/en/lessons/getting-started-with-markdown) lesson you completed at the start of the semester.)
4. Check the order and hierarchy of your code. Are all open elements closed again? Are elements nested properly? Copy and paste your TEI into [Code Beautify](https://codebeautify.org/xmlvalidator) if you'd like to check for open tags and broken elements.
5. Finally, once you're sure you've got the TEI right, link to the actual folio in the [critical edition of TCC MS O.8.35](https://cu-mkp.github.io/dyngleyfamily-editioncrafter-website/folios/#/ec) that features your transcription!

## Step 3: Explain yourself

In the same .md file, write a 4-5 paragraph blog post responding to the following questions:

- What sort of recipe did you choose, and why?
- What was the process of learning to transcribe Middle English like?
- What questions do you have about the act of recording this recipe in a manuscript?
- What aspects of the document does TEI make more visible to a future researcher?
- How does encoding the text transform its utility?
- What questions about the relationship between technical writing and making emerged in this process?


## Step 4: Submission

You'll upload your post to a new branch in our class repository just like you did last time. Name your new branch **yourname-XML** and upload your post into the **_posts** folder. Finish by submitting a **pull request** to the **_master** branch of our class repository.

## An example of the TEI markup for the first folio of the [critical edition of TCC MS O.8.35](https://cu-mkp.github.io/dyngleyfamily-editioncrafter-website/folios/#/ec):



```
<pb facs="#f016" />
<ab>
			<div>
				<head>
					<handShift/>
				<title>of all maner of Infyrmytes</title>
 					<handShift/>
 				</head>
 				<p>Here begynneth a tretys of al manere of infirmitees of mannys body. 
 				bothe withinne as touchyng to phisyke and withoute as touching to surgerie 
 				from the croune of the heed to the sool of the foot. And the remedies therwith 
 				if god wol. And furst we wol at heer of the hed how it shulde be norisshede &amp; kepte &amp;c.</p>
 			</div>
				<div>
				<head>
					<title>For to make heer to growe.</title>
				</head>
				<p>Take withien leves and sethe hem in oyle and hony and anoynte the heede 
				therwith. and it shal make the heer to growe and waxe. 
				<title>Another.</title> Take beer &amp; drie hem in a furneys or in a panne
				 and make therof a pouder. and sethe it in hony and anoynt the pacient therwith and it schal 
				 make the heer to growe. <title>Another.</title> forto make heer to growe after scalles. 
				 There is an oynement that is cleped <term>unguentum <persName>aristotilis</persName></term>. 
				 thus it must be made. Take the sewet of a dere either fresshe shepys talu and 
				 pich that is fletyng. oyle olyf and gret salt. of iche of these <measure>iii. unces</measure> 
				 or <measure>half a quartron</measure> of white waxe <measure>half an unce</measure>. 
				 than first take the sewt. or </p>
  </div>
  </ab>
```
