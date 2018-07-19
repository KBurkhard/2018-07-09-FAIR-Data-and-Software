---
layout: workshop      # DON'T CHANGE THIS.
carpentry: "swc"    # what kind of Carpentry (must be either "lc" or "dc" or "swc")
title: "FAIR Data and Software (Carpentries-based Workshop)"
venue: "Technische Informationsbibliothek (TIB)"        # brief name of host site without address (e.g., "Euphoric State University")
address: "Welfengarten 1B, 30167 Hannover, Germany"      # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria")
country: "de"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1)
language: "en"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/ISO_639-1)
latlng: "52.38151,9.72025"       # decimal latitude and longitude of workshop venue (e.g., "41.7901128,-87.6007318" - use http://www.latlong.net/)
humandate: "9-13. July 2018"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: "9:00-17:00"    # human-readable times for the workshop (e.g., "9:00 am - 4:30 pm")
startdate: 2018-07-09      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2018-07-13        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
instructor: ["Katrin Leinweber", "Angelina Kraft", "Konrad Förstner", "Martin Hammitzsch", "Luke Johnston", "Mateusz Kuzak"] # boxed, comma-separated list of instructors' names as strings, like ["Kay McNulty", "Betty Jennings", "Betty Snyder"]
helper: ["Chris Erdmann"]     # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
email: ["carpentries@tib.eu"]    # boxed, comma-separated list
collaborative_notes: https://hackmd.io/ERXxduPVTPSc3LvSjL2nfw    # https://github.com/swcarpentry/workshop-template/issues/418
---

### General Information

**This workshop aimed to train junior scientists in implementing the FAIR principles for research data & software management & development.** We want to help you identify similarities and differences between these two scientific objects and apply respectively appropriate good practices in preparing, publishing and archiving your work.

<p align="center">
<em>
  It was a new, experimental workshop format that contextualises the highly practical lesson material from the <a href="{{site.swc_site}}">Software</a> and <a href="{{site.dc_site}}">Data</a> <a href="https://carpentries.org/">Carpentries</a> with the <a href="https://blogs.tib.eu/wp/tib/2017/09/12/the-fair-data-principles-for-research-data/">FAIR principles</a>
</em>
</p>


### For whom?

Junior scientists who wish to excel at
implementing the FAIR principles for research data and scientific
software. **You need to have some previous knowledge of the tools
that will be presented at the workshop.**


### When & Where?

Please see [events.tib.eu/fair-data-software
](https://events.tib.eu/fair-data-software/)
for all the details, including public transport directions and
[accommodation suggestions](https://events.tib.eu/fair-data-software/accommodation/). You can also find us on [OpenStreetMap
](https://www.openstreetmap.org/?mlat={{page.latlng | replace:',','&mlon='}}&zoom=16)
and [add the event to your Google
Calendar](https://calendar.google.com/calendar/render?action=TEMPLATE&text=FAIR Data and Software&dates={{ page.startdate | replace: "-", "" }}/{{ page.enddate | replace: "-", "" | plus: 0}}&trp=false&sprop&sprop=name:&sf=true&output=xml&location={{ page.address }}&details="Carpentries-based workshop at the {{ page.venue }}").


### Costs

**Participation was free of charge**. However, participants needed to organise and pay for travel and [accommodation](#when--where) themselves. This workshop was part of an ideas competition supported by the [Jülich Research Centre](http://www.fz-juelich.de/portal/EN/Home/), and part of a [grant by the German Federal Ministry of Education and Research (BMBF)](https://www.bildung-forschung.digital/de/ideenwettbewerb-zum-digitalen-wandel-in-der-wissenschaft-2007.html).


### Requirements

**Please note: This workshop focussed on the application** of the FAIR Principles on scientific data and software. Because it covered a variety of examples, it did require a basic knowledge of the tools listed in [the schedule](#schedule). If you are interested in learning these basics, please consider applying for one of the (non-experimental) [Software](https://software-carpentry.org/workshops/) and [Data](http://www.datacarpentry.org/workshops-upcoming/) Carpentry workshops, or [work through](https://software-carpentry.org/lessons/) their [material](http://www.datacarpentry.org/lessons/) in a self-paced manner.


### Recordings & Workshop Material

Lectures were recorded and will be published on the [TIB AV-Portal](https://av.tib.eu/).
Slides are already available at the [TIB's NextCloud](https://tib.eu/cloud/s/tXSt3j7Bg3ySdXY).
Miscellaneous resources can also be found hyperlinked in the schedule.

### Contact

If you have any questions, please don't hesitate to [open an issue](https://github.com/TIBHannover/2018-07-09-FAIR-Data-and-Software/issues/).

---

<h2 id="schedule">Schedule</h2>

We approximately focussed on one topic / principle per day, introducing its reasoning,
benefits, and (differing and/or shared) implications for *proper research
data/software management/development* together with the learners. We
followed-up the theory-leaning introductions in the mornings with discussions and
live-coding sessions, using some (Software & Data) Carpentry materials to illustrate and
practice a principle's implementation in the
[STEM](https://en.wikipedia.org/wiki/Science,_technology,_engineering,_and_mathematics)
disciplines ("[MINT-Fächer](https://de.wikipedia.org/wiki/MINT-F%C3%A4cher)").
Regardless of discipline, learners were encouraged to **bring** questions about
their **own data and source code**, which we tried to answer during the week.

{% include schedule.html %}


### Collaborative Notes


---

## Setup

To participate in this workshop, you will need access to the software described 
below. In addition, you will need an up-to-date web browser.

We maintain a list of common issues that occur during installation as a reference 
for instructors that may be useful on the [Configuration Problems and Solutions 
wiki page]({{site.swc_github}}/workshop-template/wiki/Configuration-Problems-and-Solutions).

## Setup checklist

- [ ] [Git installed](#git)
- [ ] [text editor installed](#editor)
- [ ] [Anaconda installed](#python), Anadonda Navigator starts and  "Jupyter notebook" launches
- [ ] [RStudio installed](#r), start and `install.packages(c("ggplot2", "knitr", "pangaear", "roxygen2", "testthat", "usethis"))` worked

### Setup help

We will offer a virtual set-up help on the Thursday and Friday before the workshop
(5. & 6. of July) between 13 and 14 o'clock CEST in the afternoons ([convert to your time 
zone](https://www.timeanddate.com/worldclock/converter.html?iso=20180705T110000&p1=309)).
We'll be in the web-conference channel [meet.jit.si/FAIRDataSoftwareInstallHelp](https://meet.jit.si/FAIRDataSoftwareInstallHelp)
which should load in most modern browsers.
In order to ease debugging, please follow the [setup](#setup-details) instructions.

### Setup details

<div id="git"> {% comment %} Start of 'Git' section. GitHub browser compatability
           is given at https://help.github.com/articles/supported-browsers/{% endcomment %}
  <h3>Git</h3>
  <p>
    Git is a version control system that lets you track who made changes
    to what when and has options for easily updating a shared or public
    version of your code
    on <a href="https://github.com/">github.com</a>. You will need a
    <a href="https://help.github.com/articles/supported-browsers/">supported</a>
    web browser (current versions of Chrome, Firefox or Safari,
    or Internet Explorer version 9 or above).
  </p>
  <p>
    You will need an account at <a href="https://github.com/">github.com</a>
    for parts of the Git lesson. Basic GitHub accounts are free. We encourage
    you to create a GitHub account if you don't have one already.
    Please consider what personal information you'd like to reveal. For
    example, you may want to review these
    <a href="https://help.github.com/articles/keeping-your-email-address-private/">instructions
    for keeping your email address private</a> provided at GitHub.
  </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="git-windows">Windows</h4>
      <a href="https://www.youtube.com/watch?v=339AEqk9c-8">Video Tutorial</a>
      <ol>
        <li>Download the Git for Windows <a href="https://git-for-windows.github.io/">installer</a>.</li>
        <li>Run the installer and follow the steps bellow:
          <ol>
            {% comment %} Git 2.8.2 Setup {% endcomment %}
            {% comment %} Information {% endcomment %}
            <li>Click on "Next".</li>
            {% comment %} Select Components {% endcomment %}
            <li>Click on "Next".</li>
            {% comment %} Adjusting your PATH environment {% endcomment %}
            <li>
              <strong>
                Keep "Use Git from the Windows Command Prompt" selected and click on "Next".
              </strong>
                If you forgot to do this programs that you need for the workshop will not work properly.
                If this happens rerun the installer and select the appropriate option.
            </li>
            {% comment %} Choosing the SSH executable {% endcomment %}
            <li>Click on "Next".</li>
            {% comment %} Configuring the line ending conversions {% endcomment %}
            <li>
              <strong>
                Keep "Checkout Windows-style, commit Unix-style line endings" selected and click on "Next".
              </strong>
            </li>
            {% comment %} Configuring the terminal emulator to use with Git Bash {% endcomment %}
            <li>
              <strong>
                Keep "Use Windows' default console window" selected and click on "Next".
              </strong>
            </li>
            {% comment %} Configuring experimental performance tweaks {% endcomment %}
            <li>Click on "Install".</li>
            {% comment %} Installing {% endcomment %}
            {% comment %} Completing the Git Setup Wizard {% endcomment %}
            <li>Click on "Finish".</li>
          </ol>
        </li>
        <li>
          If your "HOME" environment variable is not set (or you don't know what this is):
          <ol>
            <li>Open command prompt (Open Start Menu then type <code>cmd</code> and press [Enter])</li>
            <li>
              Type the following line into the command prompt window exactly as shown:
              <p><code>setx HOME "%USERPROFILE%"</code></p>
            </li>
            <li>Press [Enter], you should see <code>SUCCESS: Specified value was saved.</code></li>
            <li>Quit command prompt by typing <code>exit</code> then pressing [Enter]</li>
          </ol>
        </li>
      </ol>
      <p>This will provide you with both Git and Bash in the Git Bash program.</p>
    </div>
    <div class="col-md-4">
      <h4 id="git-macosx">macOS</h4>
      <a href="https://www.youtube.com/watch?v=9LQhwETCdwY ">Video Tutorial</a>
      <p>
        <strong>For OS X 10.9 and higher</strong>, install Git for Mac
        by downloading and running the most recent "mavericks" installer from
        <a href="http://sourceforge.net/projects/git-osx-installer/files/">this list</a>.
        After installing Git, there will not be anything in your <code>/Applications</code> folder,
        as Git is a command line program.
        <strong>For older versions of OS X (10.5-10.8)</strong> use the
        most recent available installer labelled "snow-leopard"
        <a href="http://sourceforge.net/projects/git-osx-installer/files/">available here</a>.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="git-linux">Linux</h4>
      <p>
        If Git is not already available on your machine you can try to
        install it via your distro's package manager. For Debian/Ubuntu run
        <code>sudo apt-get install git</code> and for Fedora run
        <code>sudo dnf install git</code>.
      </p>
    </div>
  </div>
</div> {% comment %} End of 'Git' section. {% endcomment %}

<div id="editor"> {% comment %} Start of 'editor' section. {% endcomment %}
  <h3>Text Editor</h3>

  <p>
    When you're writing code, it's nice to have a text editor that is
    optimized for writing code, with features like automatic
    color-coding of key words.  The default text editor on macOS and
    Linux is usually set to Vim, which is not famous for being
    intuitive.  If you accidentally find yourself stuck in it, try
    typing the escape key, followed by <code>:q!</code> (colon, lower-case 'q',
    exclamation mark), then hitting Return to return to the shell.
  </p>
  
  <p>
    <strong>If you do not already use a text editor</strong> like 
    <a href="https://notepad-plus-plus.org/">Notepad++</a> (Windows),
    <a href="https://wiki.gnome.org/Apps/Gedit">Gedit</a> or
    <a href="https://kate-editor.org/">Kate</a> (Linux),
    <a href="https://www.barebones.com/products/textwrangler/">Text Wrangler</a> or 
    <a href="https://www.barebones.com/products/bbedit/">BBEdit</a> (macOS),
    <a href="https://www.sublimetext.com/">Sublime Text</a>,
    or are already comfortable with any other, <strong>please install
    <a href="https://atom.io/">Atom</a></strong>.
  </p>
  
  <p>
    In any case, please configure Git to use one of them, by applying the
    <a href="https://swcarpentry.github.io/git-novice/02-setup/">
    specific <code>core.editor</code> configuration command
    from the Software Carpentry's "Git Novice" lesson</a>.
  </p>
  
</div> {% comment %} End of 'editor' section. {% endcomment %}

<div id="python"> {% comment %} Start of 'Python' section. Remove the third paragraph if
           the workshop will teach Python using something other than
           the Jupyter notebook.
           Details at https://jupyter-notebook.readthedocs.io/en/stable/notebook.html#browser-compatibility {% endcomment %}
  <h3>Python</h3>

  <p>
    <a href="https://python.org">Python</a> is a popular language for
    research computing, and great for general-purpose programming as
    well.  Installing all of its research packages individually can be
    a bit difficult, so we recommend
    <a href="https://www.anaconda.com/distribution/">Anaconda</a>,
    an all-in-one installer.
  </p>

    <p>
      Regardless of how you choose to install it,
      <strong>please make sure you install Python version 3.x</strong>
      (e.g., 3.6 is fine).
    </p>

    <p>
      We will teach Python using the <a href="https://jupyter.org/">Jupyter notebook</a>,
      a programming environment that runs in a web browser. For this to work you will need a reasonably
      up-to-date browser. The current versions of the Chrome, Safari and
      Firefox browsers are all
      <a href="https://jupyter-notebook.readthedocs.io/en/stable/notebook.html#browser-compatibility">supported</a>
      (some older browsers, including Internet Explorer version 9
      and below, are not).
    </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="python-windows">Windows</h4>
      <a href="https://www.youtube.com/watch?v=xxQ0mzZ8UvA">Video Tutorial</a>
      <ol>
        <li>Open <a href="https://www.anaconda.com/download/#windows">https://www.anaconda.com/download/#windows</a> with your web browser.</li>
        <li>Download the Python 3 installer for Windows.</li>
        <li>Install Python 3 using all of the defaults for installation <em>except</em> make sure to check <strong>Make Anaconda the default Python</strong>.</li>
      </ol>
    </div>
    <div class="col-md-4">
      <h4 id="python-macosx">macOS</h4>
      <a href="https://www.youtube.com/watch?v=TcSAln46u9U">Video Tutorial</a>
      <ol>
        <li>Open <a href="https://www.anaconda.com/download/#macos">https://www.anaconda.com/download/#macos</a> with your web browser.</li>
        <li>Download the Python 3 installer for macOS.</li>
        <li>Install Python 3 using all of the defaults for installation.</li>
      </ol>
    </div>
    <div class="col-md-4">
      <h4 id="python-linux">Linux</h4>
      <ol>
        <li>Open <a href="https://www.anaconda.com/download/#linux">https://www.anaconda.com/download/#linux</a> with your web browser.</li>
        <li>Download the Python 3 installer for Linux.<br>
          (The installation requires using the shell. If you aren't
           comfortable doing the installation yourself
           stop here and request help at the workshop.)
        </li>
        <li>
          Open a terminal window.
        </li>
        <li>
          Type <pre>bash Anaconda3-</pre> and then press
          tab. The name of the file you just downloaded should
          appear. If it does not, navigate to the folder where you
          downloaded the file, for example with:
          <pre>cd Downloads</pre>
          Then, try again.
        </li>
        <li>
          Press enter. You will follow the text-only prompts. To move through
          the text, press the space key. Type <code>yes</code> and
          press enter to approve the license. Press enter to approve the
          default location for the files. Type <code>yes</code> and
          press enter to prepend Anaconda to your <code>PATH</code>
          (this makes the Anaconda distribution the default Python).
        </li>
        <li>
          Close the terminal window.
        </li>
      </ol>
    </div>
  </div>
{% comment %}
  <p>
  Once you are done installing the software listed above,
  please go to <a href="setup/index.html">this page</a>,
  which has instructions on how to test that everything was installed correctly.
  </p>
{% endcomment %}
</div> {% comment %} End of 'Python' section. {% endcomment %}

<div id="r"> {% comment %} Start of 'R' section. {% endcomment %}
  <h3>R</h3>

  <p>
    <a href="https://www.r-project.org">R</a> is a programming language
    that is especially powerful for data exploration, visualization, and
    statistical analysis. To interact with R, we use
    <a href="https://www.rstudio.com/">RStudio</a>.
  </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="r-windows">Windows</h4>
      <a href="https://www.youtube.com/watch?v=q0PjTAylwoU">Video Tutorial</a>
      <p>
        Install R by downloading and running
        <a href="https://cran.r-project.org/bin/windows/base/release.htm">this .exe file</a>
        from <a href="https://cran.r-project.org/index.html">CRAN</a>.
        Then, install <a href="https://www.rstudio.com/products/rstudio/download/#download">RStudio Desktop</a>.
        Note that if you have separate user and admin accounts, you should run the 
        installers as administrator (right-click on .exe file and select "Run as 
        administrator" instead of double-clicking). Otherwise problems may occur later, 
        for example when installing R packages.
	      Because you'll also be learning to <em>build</em> R packages, please also install the
	      <a href="https://ftp.gwdg.de/pub/misc/cran/bin/windows/Rtools/">Rtools</a>.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="r-macosx">macOS</h4>
      <a href="https://www.youtube.com/watch?v=5-ly3kyxwEg">Video Tutorial</a>
      <p>
        Install R by downloading and running
        <a href="https://cran.r-project.org/bin/macosx/R-latest.pkg">this .pkg file</a>
        from <a href="https://cran.r-project.org/index.html">CRAN</a>.
        Then, install <a href="https://www.rstudio.com/products/rstudio/download/#download">RStudio Desktop</a>.
	      Because you'll also be learning to <em>build</em> R packages, please also install 
	      <a href="https://ftp.gwdg.de/pub/misc/cran/bin/macosx/tools/"><code>clang-6...pkg</code>
	      and <code>gfortran-6...pkg</code></a>.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="r-linux">Linux</h4>
      <p>
        You can download the binary files for your distribution
        from <a href="https://cran.r-project.org/index.html">CRAN</a>. Or
        you can use your package manager (e.g. for Debian/Ubuntu
        run <code>sudo apt-get install r-base</code> and for Fedora run
        <code>sudo dnf install R</code>).  Also, please install the
        <a href="https://www.rstudio.com/products/rstudio/download/#download">RStudio Desktop</a>.
      </p>
    </div>
  </div>
  <p>
    Please also run the following installation command in your R console before
    attending:
  <code>
    install.packages(c("ggplot2", "knitr", "pangaear", "roxygen2", "testthat", "usethis"))
    </code>
  </p>
</div> {% comment %} End of 'R' section. {% endcomment %}

We used a <a href="{{page.collaborative_notes}}">HackMD.io pad</a> to share URLs, bits of code, and to take notes.

[![](fig/footer_logos.png)](https://events.tib.eu/fair-data-software/)
