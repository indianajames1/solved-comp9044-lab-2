Download Link: https://assignmentchef.com/product/solved-comp9044-lab-2
<br>



Before the lab you should re-read the relevant lecture slides and their accompanying examples.

Create a new directory for this lab called lab02, change to this directory, and fetch the provided code for this week by running these commands:

$ <strong>mkdir lab02</strong>

$ <strong>cd lab02</strong>

$ <strong>2041 fetch lab02</strong>

Or, if you’re not working on CSE, you can download the provided code as a <a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/lab/02/provided.zip">zip</a> <a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/lab/02/provided.zip">file</a> or a <a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/lab/02/provided.tar">tar</a> <a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/lab/02/provided.tar">file</a>.

There is a template file named counting_classes_answers.txt which you must use to enter the answers for this exercise.

Download <a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/activities/counting_classes/counting_classes_answers.txt">countin</a><a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/activities/counting_classes/counting_classes_answers.txt">g</a><a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/activities/counting_classes/counting_classes_answers.txt">_</a><a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/activities/counting_classes/counting_classes_answers.txt">classes</a><a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/activities/counting_classes/counting_classes_answers.txt">_</a><a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/activities/counting_classes/counting_classes_answers.txt">answers</a><a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/activities/counting_classes/counting_classes_answers.txt">.</a><a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/activities/counting_classes/counting_classes_answers.txt">txt</a><a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/activities/counting_classes/counting_classes_answers.txt">,</a> or copy it to your CSE account using the following command:

$ <strong>cp -n /web/cs2041/20T2/activities/counting_classes/counting_classes_answers.txt .</strong>

The autotest scripts depend on the format of counting_classes_answers.txt so just add your answers don’t otherwise change the file. In other words edit <sub>counting_classes_answers.txt</sub>:

<strong>gedit counting_classes_answers.txt &amp;</strong>

The file classes.txt contains a list of CSE classes downloaded from myUNSW.

Download <a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/activities/counting_classes/classes.txt">classes</a><a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/activities/counting_classes/classes.txt">.</a><a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/activities/counting_classes/classes.txt">txt</a>, or copy it to your CSE account using the following command:

$ <strong>cp -n /web/cs2041/20T2/activities/counting_classes/classes.txt .</strong>




. Write a shell pipeline to print how many classes there are. Hint: the output of the pipeline should be:

441

. Write a shell pipeline to print how many different courses have classes. Hint: cut with the -f option will be useful here.

Hint: the output of the pipeline should be:

35

. Write a shell pipeline which will print the course with the most classes (and no other courses) and how many classes are in this course.

Hint: the output of the pipeline should be:

31 COMP1521

. Write a shell pipeline that prints the room most frequently-used room by CSE classes and how often it is used. Don’t include the CSE lab rooms.

Hint: the output of the pipeline should be:

26 Quad 1042

. Write a shell pipeline that prints the most common day and hour in the week for classes to start and how many classes start at that time.

Hint: cut has a -c option.

Hint: the output of the pipeline should be:

20 Fri 11

. Challenge: Write a shell pipeline that prints a list of the course codes (only) of COMP courses that run 2 or more classes of the same type starting at the same time on the same day (e.g. three tut-labs starting Monday at 10 00). Hint: this should be the output of your pipeline:

COMP1000

COMP1511

COMP1521

COMP2041

COMP2511

COMP2521

COMP3331

COMP6441

COMP6841

COMP9044

COMP9311

COMP9313

COMP9331

COMP9417

When you think your program is working, you can use autotest to run some simple automated tests:

$ <strong>2041 autotest counting_classes</strong>

<h1>Autotest Results</h1>

77% of 572 students who have autotested counting_classes_answers.txt so far, passed all autotest tests. 99% passed test <em>q1</em> <em>q2</em> <em>q3</em> <em>q4</em>

98% passed test <em>q5</em>

80% passed test <em>q6</em>

When you are finished working on this exercise, you must submit your work by running give:

$ <strong>give cs2041 lab02_counting_classes counting_classes_answers.txt</strong>

before Tuesday 16 June 17 59 to obtain the marks for this lab exercise.

Write a program digits.sh that reads from standard input and writes to standard output mapping all digit characters whose values are less than 5 into the character ‘<sub>&lt;</sub>‘ and all digit characters whose values are greater than 5 into the character ‘<sub>&gt;</sub>‘. The digit character ‘5’ should be left unchanged.

<table width="670">

 <tbody>

  <tr>

   <td width="335">Sample Input Data</td>

   <td width="335">Corresponding Output</td>

  </tr>

  <tr>

   <td width="335">


    <table width="321">

     <tbody>

      <tr>

       <td width="321">1 234 5 678 9</td>

      </tr>

     </tbody>

    </table></td>

   <td width="335">


    <table width="321">

     <tbody>

      <tr>

       <td width="321">&lt; &lt;&lt;&lt; 5 &gt;&gt;&gt; &gt;</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

  <tr>

   <td width="335">


    <table width="321">

     <tbody>

      <tr>

       <td width="321">I can think of 100’s of other things I’d rather be doing than these 3 questions</td>

      </tr>

     </tbody>

    </table></td>

   <td width="335">


    <table width="321">

     <tbody>

      <tr>

       <td width="321">I can think of &lt;&lt;&lt;‘s of other things I’d rather be doing than these &lt; questions</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

  <tr>

   <td width="335">


    <table width="321">

     <tbody>

      <tr>

       <td width="321">A line with lots of numbers:123456789123456789123456789A line with all zeroes000000000000000000000000000A line with blanks at the end1 2 3</td>

      </tr>

     </tbody>

    </table></td>

   <td width="335">


    <table width="321">

     <tbody>

      <tr>

       <td width="321">A line with lots of numbers:&lt;&lt;&lt;&lt;5&gt;&gt;&gt;&gt;&lt;&lt;&lt;&lt;5&gt;&gt;&gt;&gt;&lt;&lt;&lt;&lt;5&gt;&gt;&gt;&gt;A line with all zeroes&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt;A line with blanks at the end&lt; &lt; &lt;</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

  <tr>

   <td width="335">


    <table width="321">

     <tbody>

      <tr>

       <td width="321">Input with absolutely 0 digits in it Well … apart from that one …</td>

      </tr>

     </tbody>

    </table></td>

   <td width="335">


    <table width="321">

     <tbody>

      <tr>

       <td width="321">Input with absolutely &lt; digits in it Well … apart from that one …</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

  <tr>

   <td width="335">


    <table width="321">

     <tbody>

      <tr>

       <td width="321">1 2 4 8 16 32 64 128 256 512 10242048 4096 8192 16384 32768 65536</td>

      </tr>

     </tbody>

    </table></td>

   <td width="335">


    <table width="321">

     <tbody>

      <tr>

       <td width="321">&lt; &lt; &lt; &gt; &lt;&gt; &lt;&lt; &gt;&lt; &lt;&lt;&gt; &lt;5&gt; 5&lt;&lt; &lt;&lt;&lt;&lt;&lt;&lt;&lt;&gt; &lt;&lt;&gt;&gt; &gt;&lt;&gt;&lt; &lt;&gt;&lt;&gt;&lt; &lt;&lt;&gt;&gt;&gt; &gt;55&lt;&gt;</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

Hint: tr can be used.

When you think your program is working, you can use autotest to run some simple automated tests:

$ <strong>2041 autotest digits</strong>

<h1>Autotest Results</h1>

99% of 557 students who have autotested digits.sh so far, passed all autotest tests.  99% passed test <em>1</em> <em>2</em> <em>3</em> <em>4</em> <em>5</em>

When you are finished working on this exercise, you must submit your work by running give:

$ <strong>give cs2041 lab02_digits digits.sh</strong>

before Tuesday 16 June 17 59 to obtain the marks for this lab exercise.

Write a shell script called echon.sh which given exactly two arguments, an integer <em>n</em> and a string, prints the string <em>n</em> times. For example:

<table width="961">

 <tbody>

  <tr>

   <td width="961"><strong>./echon.sh 5 hello</strong> hello hello hello hello hello<strong>./echon.sh 0 nothing ./echon.sh 1 goodbye</strong> goodbye</td>

  </tr>

 </tbody>

</table>

Your script should print exactly the error message below if it is not given exactly 2 arguments:

<strong>./echon.sh </strong>

Usage: ./echon.sh &lt;number of lines&gt; &lt;string&gt; <strong>./echon.sh 1 2 3</strong>

Usage: ./echon.sh &lt;number of lines&gt; &lt;string&gt;

Also get your script to print this error message if its first argument isn’t a non-negative integer:

<strong>./echon.sh hello world</strong>

./echon.sh: argument 1 must be a non-negative integer <strong>./echon.sh -42 lines</strong>

./echon.sh: argument 1 must be a non-negative integer

Although its better practice to print your error messages to stderr its OK to print your error messages to stdout for this exercise.

Hint: you’ll need to use the shell if, while and exit statements, shell arithmetic and the test command.

When you think your program is working, you can use autotest to run some simple automated tests:

$ <strong>2041 autotest echon</strong>

<h1>Autotest Results</h1>

95% of 553 students who have autotested echon.sh so far, passed all autotest tests.

99% passed test <em>1</em>

100% passed test <em>2</em>

100% passed test <em>2</em>

99% passed test <em>3</em> <em>4</em> <em>5</em> <em>6</em>

96% passed test <em>7</em>

98% passed test <em>8</em>

When you are finished working on this exercise, you must submit your work by running give:

$ <strong>give cs2041 lab02_echon echon.sh</strong>

before Tuesday 16 June 17 59 to obtain the marks for this lab exercise.

Write a shell script file_sizes.sh which prints the names of the files in the current directory splitting them into three categories: <em>small</em>, <em>medium-sized</em> and <em>large</em>. A file is considered <em>small</em> if it contains less than 10 lines, <em>medium-sized</em> if contains less than 100 lines, otherwise it is considered <em>large</em>.

Your script should always print exactly three lines of output. Files should be listed in alphabetic order on each line. Your shell-script should match character-for-character the output shown in the example below. Notice the creation of a separate direcory for testing and the use of the script from the last question to produce test files. You could also produce test files manually using an editor.

<table width="961">

 <tbody>

  <tr>

   <td width="961"><strong>mkdir test cd test ../echon.sh 5 text &gt;a</strong><strong>../echon.sh 505 text &gt;bbb</strong><strong>../echon.sh 17 text &gt;cc</strong><strong>../echon.sh 10 text &gt;d</strong><strong>../echon.sh 1000 text &gt;e ../echon.sh 0 text &gt;empty ls -l</strong> total 24-rw-r–r– 1 andrewt andrewt   25 Mar 24 10:37 a-rw-r–r– 1 andrewt andrewt 2525 Mar 24 10:37 bbb-rw-r–r– 1 andrewt andrewt   85 Mar 24 10:37 cc-rw-r–r– 1 andrewt andrewt   50 Mar 24 10:37 d-rw-r–r– 1 andrewt andrewt 5000 Mar 24 10:37 e-rw-r–r– 1 andrewt andrewt    0 Mar 24 10:37 empty<strong>../file_sizes.sh </strong>Small files: a emptyMedium-sized files: cc d Large files: bbb e <strong>rm cc d ../echon.sh 10000 . &gt;lots_of_dots ls -l</strong> total 36-rw-r–r– 1 andrewt andrewt    25 Mar 24 10:37 a-rw-r–r– 1 andrewt andrewt  2525 Mar 24 10:37 bbb-rw-r–r– 1 andrewt andrewt  5000 Mar 24 10:37 e-rw-r–r– 1 andrewt andrewt     0 Mar 24 10:37 empty-rw-r–r– 1 andrewt andrewt 20000 Mar 24 10:39 lots_of_dots<strong>../file_sizes.sh </strong> Small files: a empty Medium-sized files:Large files: bbb e lots_of_dots</td>

  </tr>

 </tbody>

</table>

Hint: you can use the command <sub>wc</sub> to discover how many lines are in a file. You probably want to use the shell’s back quotes, its <sub>if </sub>statement, and the test command.

When you think your program is working, you can use autotest to run some simple automated tests:

$ <strong>2041 autotest file_sizes</strong>

<h1>Autotest Results</h1>

98% of 527 students who have autotested file_sizes.sh so far, passed the autotest test.

When you are finished working on this exercise, you must submit your work by running give:

$ <strong>give cs2041 lab02_file_sizes file_sizes.sh</strong>

before Tuesday 16 June 17 59 to obtain the marks for this lab exercise.

Write a shell script scraping_courses.sh which prints a list of UNSW courses with the given prefix by extracting them from the 2018 UNSW handbook webpages.

This year UNSW has changed to much prettier format but also a format which it is much harder for a script to extract information from.

So for this exercise we’ll use the 2018 handbook pages which aren’t For example:




<table width="961">

 <tbody>

  <tr>

   <td width="961"><strong>scraping_courses.sh OPTM</strong>OPTM2111 Optometry 2AOPTM2133 The Clinical EnvironmentOPTM2190 Introduction to Clinical OptometryOPTM2211 Optometry 2BOPTM2233 Optical DispensingOPTM2291 Primary Care OptometryOPTM3105 Disease Processes of the Eye 1OPTM3111 Optometry 3AOPTM3131 Ocular Disease 3AOPTM3133 Vision Science in the Consulting RoomOPTM3201 Ocular Imaging &amp; Applied Vision Science OPTM3205 Disease Processes of the Eye 2OPTM3211 Optometry 3BOPTM3231 Ocular Disease 3BOPTM3233 Working in the clinical environmentOPTM4110 Optometry 4AOPTM4131 Clinical Optometry 4AOPTM4151 Ocular Therapeutics 4AOPTM4211 Optometry 4BOPTM4231 Clinical Optometry 4BOPTM4251 Ocular Therapeutics 4BOPTM4271 Professional OptometryOPTM4291 Optometry, Medicine &amp; Patient ManagementOPTM5111 Clinical Optometry 5AOPTM5131 Specialist Clinical Optometry 5AOPTM5151 Clinical Ocular Therapeutics 5AOPTM5171 Research Project 5AOPTM5211 Clinical Optometry 5BOPTM5231 Specialist Clinical Optometry 5BOPTM5251 Clinical Ocular Therapeutics 5B OPTM5271 Research Project 5BOPTM6400 Optometric Preclinical PracticeOPTM6411 Contact LensesOPTM6412 Clinical Optometry 4AOPTM6413 Anterior Eye TherapeuticsOPTM6421 Binocular Vision, Paediatrics and Low VisionOPTM6422 Clinical Optometry 4BOPTM6423 Therapeutics and the Posterior EyeOPTM6424 Professional OptometryOPTM7001 Introduction to Community Eye HealthOPTM7002 Epidemiology &amp; Biostatistics for Needs AssessmentOPTM7003 Epidemiology of Blinding Eye DiseasesOPTM7004 Advocacy and Education in Community Eye Health OPTM7005 Eye Health Economics and SustainabilityOPTM7006 Eye Care Program ManagementOPTM7007 Community Eye Health ProjectOPTM7103 Behavioural Optometry 1OPTM7104 Advanced Contact Lens Studies 1OPTM7108 Research Skills in OptometryOPTM7110 Public Health OptometryOPTM7115 Visual NeuroscienceOPTM7117 Ocular Therapy 2OPTM7203 Behavioural Optometry 2 OPTM7205 Specialty Contact Lens StudiesOPTM7213 Ocular TherapyOPTM7301 Advanced Clinical OptometryOPTM7302 Evidence Based OptometryOPTM7308 Research ProjectOPTM7444 Business Skills in OptometryOPTM7511 Advanced Ocular Disease 1OPTM7521 Advanced Ocular Disease 2OPTM8511 Clinical paediatrics, low vision and colour visionOPTM8512 Clinical Optometry 5AOPTM8513 Clinical Ocular Therapy 5AOPTM8518 Optometry Research Project AOPTM8521 Clinical Contact LensesOPTM8522 Clinical Optometry 5BOPTM8523 Clinical Ocular Therapy 5B OPTM8528 Optometry Research Project B <strong>scraping_courses.sh MATH|wc</strong></td>

  </tr>

  <tr>

   <td width="961">    126     585    4874<strong>scraping_courses.sh COMP|grep Soft</strong>COMP1531 Software Engineering FundamentalsCOMP2041 Software Construction: Techniques and ToolsCOMP3141 Software System Design and ImplementationCOMP3431 Robotic Software ArchitectureCOMP4161 Advanced Topics in Software VerificationCOMP4181 Language-based Software SafetyCOMP6447 System and Software Security AssessmentCOMP9041 Software Construction: Techniques and ToolsCOMP9181 Language-based Software Safety COMP9322 Software Service Design and EngineeringCOMP9323 Software as a Service Project COMP9431 Robotic Software Architecture <strong>scraping_courses.sh MINE|grep Rock</strong>MINE3630 Rock BreakageMINE8640 Geotechnical Hazards in Hard Rock MinesMINE8660 Geotechnical Engineering for Underground Hard Rock</td>

  </tr>

 </tbody>

</table>

Your script must download the handbook web pages and extract the information from them when it is run.

<h1>Hints</h1>

This task can be done using the usual tools of egrep, sed, sort &amp; uniq but the regular expressions take some thought.

The UNSW handbook uses seperate web pages for undergraduate and postgraduate courses. These two web pages would need to be downloaded for the above example (OPTM):

<a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Undergraduate&amp;descr=O">http://le</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Undergraduate&amp;descr=O">g</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Undergraduate&amp;descr=O">ac</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Undergraduate&amp;descr=O">y</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Undergraduate&amp;descr=O">.handbook.unsw.edu.au/vbook2018/brCoursesB</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Undergraduate&amp;descr=O">y</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Undergraduate&amp;descr=O">AtoZ.</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Undergraduate&amp;descr=O">j</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Undergraduate&amp;descr=O">sp?Stud</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Undergraduate&amp;descr=O">y</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Undergraduate&amp;descr=O">Level=Under</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Undergraduate&amp;descr=O">g</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Undergraduate&amp;descr=O">raduate&amp;descr=O</a> and <a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">http://le</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">g</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">ac</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">y</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">.handbook.unsw.edu.au/vbook2018/brCoursesB</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">y</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">AtoZ.</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">j</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">sp?Stud</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">y</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">Level=Post</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">g</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">raduate&amp;descr=O</a><a href="http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?StudyLevel=Postgraduate&amp;descr=O">. </a>Make sure courses which occur in both postgraduate &amp; undergraduate handbooks aren’t repeated. cat -A can be useful to check for non-printing characters.

The command curl will download a URL and print it to standard output.

In a script it is best run as curl –silent so it doesn’t print extra information on standard error.

For example:

<table width="961">

 <tbody>

  <tr>

   <td width="961"><strong>curl –silent “http://legacy.handbook.unsw.edu.au/vbook2018/brCoursesByAtoZ.jsp?</strong><strong>StudyLevel=Undergraduate&amp;descr=O”|grep OPTM</strong>&lt;TD class=”” align=”left”&gt;OPTM2111&lt;/TD&gt;&lt;TD class=””&gt;&lt;A href=”http://www.handbook.unsw.edu.au/undergraduate/courses/2018/OPTM2111.html”&gt;Optometry 2A&lt;/A&gt;&lt;/TD&gt;&lt;TD class=”evenTableCell” align=”left”&gt;OPTM2133&lt;/TD&gt;&lt;TD class=”evenTableCell”&gt;&lt;Ahref=”http://www.handbook.unsw.edu.au/undergraduate/courses/2018/OPTM2133.html”&gt;The Clinical Environment &lt;/A&gt; &lt;/TD&gt;&lt;TD class=”” align=”left”&gt;OPTM2190&lt;/TD&gt;&lt;TD class=””&gt;&lt;Ahref=”http://www.handbook.unsw.edu.au/undergraduate/courses/2018/OPTM2190.html”&gt;Introduction to Clinical Optometry &lt;/A&gt;&lt;/TD&gt;&lt;TD class=”evenTableCell” align=”left”&gt;OPTM2211&lt;/TD&gt;&lt;TD class=”evenTableCell”&gt;&lt;A href=”http://www.handbook.unsw.edu.au/undergraduate/courses/2018/OPTM2211.html”&gt;Optometry 2B&lt;/A&gt;&lt;/TD&gt;                                 &lt;TD class=”” align=”left”&gt;OPTM2233&lt;/TD&gt;&lt;TD class=””&gt;&lt;A href=”http://www.handbook.unsw.edu.au/undergraduate/courses/2018/OPTM2233.html”&gt;Optical Dispensing &lt;/A&gt;&lt;/TD&gt; …</td>

  </tr>

 </tbody>

</table>

The program wget can be used for the same purpose, by running it as wget -q -O- <em>url</em>

When you think your program is working, you can use autotest to run some simple automated tests:

$ <strong>2041 autotest scraping_courses</strong>

<h1>Autotest Results</h1>

82% of 190 students who have autotested scraping_courses.sh so far, passed all autotest tests. 91% passed test <em>1</em>

84% passed test <em>2</em>

87% passed test <em>3</em>

88% passed test <em>4</em>

86% passed test <em>5</em>

When you are finished working on this exercise, you must submit your work by running give:

$ <strong>give cs2041 lab02_scraping_courses scraping_courses.sh</strong>

before Tuesday 16 June 17 59 to obtain the marks for this lab exercise.

When you are finished each exercises make sure you submit your work by running give.

You can run give multiple times. Only your last submission will be marked.

Don’t submit any exercises you haven’t attempted.

If you are working at home, you may find it more convenient to upload your work via <a href="https://cgi.cse.unsw.edu.au/~give/Student/give.php">g</a><a href="https://cgi.cse.unsw.edu.au/~give/Student/give.php">ive</a><a href="https://cgi.cse.unsw.edu.au/~give/Student/give.php">‘</a><a href="https://cgi.cse.unsw.edu.au/~give/Student/give.php">s</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/give.php">web</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/give.php">interface</a><a href="https://cgi.cse.unsw.edu.au/~give/Student/give.php">.</a>

Remember you have until Tuesday 16 June 17 59 59 to submit your work.

You cannot obtain marks by e-mailing your code to tutors or lecturers.

You check the files you have submitted <a href="https://cgi.cse.unsw.edu.au/~cs2041/20T2/student/">here</a>.

Automarking will be run by the lecturer several days after the submission deadline, using test cases different to those autotest runs for you. (Hint: do your own testing as well as running autotest.)

<a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">After</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">automarking</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">is</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">run</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">by</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">the</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">lecturer</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">you</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">can</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">view</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">y</a><a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">our</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">results</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">here</a><a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">.</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">The</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">resulting</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">mark</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">will</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">also</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">be</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">available</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">via</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">g</a><a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">ive</a><a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">‘</a><a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">s</a> <a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">web interface</a><a href="https://cgi.cse.unsw.edu.au/~give/Student/sturec.php">.</a>