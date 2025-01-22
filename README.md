java c
Department of Computer Science 
Summative Coursework Set FrontPage 
Module Title 
Applied Data Science with Python 
Module Code 
CSMAD 
Type of Assignment 
(e.g., technical report, set exercise, in-class test) 
Set exercise 2 of 2 
Individual or Group Assignment 
Individual 
Weighting of the Assignment 
50% 
Word count/page limit 
Approximately 1,500 words, excluding code, code comments, captions and 
tables. 
Expected hrs spent for the assignment (set by lecturer) 
20 



Items to be submitted 
A single .zip archive, containing: 
1. All final project code. 
2. One fully executed Jupyter 
Notebook file (.ipynb), displaying code, figures, and explanations (as Markdown) 
3. One HTML file (.html), exported from above Jupyter Notebook. 
Work to be submitted on-line via Blackboard Learn by 
Monday, 27 January 2025, 12:00 noon 
Work will be marked and returned by 
Friday, 14 February 2025 
1. Assessment classifications 
This coursework assesses   your   ability to:
•          acquire       and       be       able       to       apply      statistical,       programming,      and       machine       learning   techniques   in   Python for data science tasks;
•          evaluate,   select   and   use   state-of-the-art   Python   tools   and   platforms   for   solving   data   science   problems;
•          design,   implement, and   execute solutions   in   Python   for   data   science   problems;   and
•          evaluate       data       science       solutions       in       Python,       including       their       outcomes,      efficacy,   constraints, and   uncertainty.
You will gain   credit for:
•          preparing   and submitting   required   files   as   requested;
•          successful   implementation of the   requested coding tasks;
•          writing   efficient, functional   code;
•          providing thoughtful, clear,   well-structured   written   analysis.Your   assignment   will   be   marked   according   to   the   marking   schemes   provided   below.   The   schemes   are   designed   so   that   the   collectively   weighted   assignment    mark   will   correspond   to   the   following   qualitative    master’s    degree   classification   descriptions.   The   table   below   describes   what   is   typically   expected   of   the   work   to   obtain   a   given   mark.
Classification Range 
Typically, the work should meet these requirements 
Distinction (>=70%) Outstanding/excellent    work with    correct codes and results. An outstanding work should demonstrate coding proficiency with high efficiency    and    based    on    advanced    techniques.    Written analyses demonstrate    exceptional       understanding    and application    of the related concepts and techniques, with focused attention to details of the    results.       The    work exhibits originality and    includes critical analysis. 
Merit (60-69%) Good work with mostly correct results: most work has been carried out    correctly.    Some tasks    have    not    been    carried    out    or    are    not completely correct.             Coding with average efficiency.             Written analyses show a strong    understanding of the subject, with clear application of sensibly chosen concepts and techniques.    The work includes some critical evaluation and broad generalization of the results. 
Pass (50-59%) Achievement of the minimum requirements. Some significant part of the assignment is missing and/or has    partially correct    results. Coding       lacks          efficiency.                   Written       analyses          meet          the       basic requirements,          demonstrating             adequate             understanding             and applications of key concepts, but the work may lack depth, contain technical errors, omit specific discussion of the results, or include improperly selected techniques. 
Fail (<50%) Incomplete solutions to limited part of the assignment. Most tasks have not been carried out with sufficient accuracy.    Results may not be    correct    or    technically    sound.          Coding    is inefficient.          Written analyses do not meet the required standards, demonstrating insufficient understanding. Work ignores consideration of specific results and is missing key components. 
2. Assignment description 
Data Description The   data   for   this   coursework   are   available   in   a   single CSMAD_CW2_data.zip file   on the CSMAD   Blackboard   space,   under the Assessment heading, Coursework 2 of 2.    You MUST use this version   of the datasets.    The archive   is   organized   as   shown:CSMAD_CW2_data.zip └── data/ ├── traffic/ │ ├── DailyStandard_Report_1_19078_01_01_2021 … .csv │ ├── ... intermediate files ... │ ├── DailyStandard_Report_1_19124_01_01_2024 … .csv │ └── TRIS+-+User+Guide+r3.pdf └── weather/ ├── 03761099999_2021.csv ├── 03761099999_2022.csv ├── 03761099999_2023.csv ├── 03761099999_2024.csv ├── CSV_HELP.pdf └── isd-format-document.pdf 
Vehicle Traffic Data: traffic/ The traffic directory contains eight CSV files.   These   Daily   Standard Reports describe   the flow of traffic   past two   Motorway   Incident   Detection and Automated Signalling   (MIDAS) observing stations on the   M4, south of   Reading.    Most column headers   are   self-explanatory.    To   clarify   other   column   headers,   those   with cm units   record   the   count   of vehicles   of   a   size   (length)   within the   stated   range, those with mph ranges   are    missing, Avg mph is    the    recorded    average    speed    of      vehicles,      and Total Volume is the   count of all vehicles during the   preceding   15   minutes.
The   TRIS+-+User+Guide+r3.pdf   file   describes   datasets   from   which   the   CSV   data is   sourced.    While this   is   included   largely for   informational   purposes,   you will   need   to   reference the definition   of Day Type for some   portions of   this   coursework.
Source:https://webtris.highwaysengland.co.uk/ 
Weather Data: weather/ The   weather   directory   contains   four   CSV   files.      These   describe   common   weather   observations   at   a   location   near those   of the   above   MIDAS   observing   stations.    The   definition   of   the   data   in   these   files   is NOT made   obvious   by   the   column   headers.   Instead,   elements   of   this   c代 写CSMAD Applied Data Science with PythonPython
代做程序编程语言oursework   will   require   that   you   use   the   CSV_HELP.pdf and   isd-format-document.pdf   files to   understand   and decode the   existing   data   representations.      Make   special   note   that   you   will   need to   choose   between   FM-12   and   FM-15 report types.
Source:
https://www.ncei.noaa.gov/metadata/geoportal/rest/metadata/item/gov.noaa.n cdc:C00532/html
Coursework Task: Analysing and Predicting Traffic Flow Using Regression and Time Series Models In   this   coursework,   students   will   develop   a   data   science   project   aimed   at   predicting   traffic flow using historical traffic and weather data spanning   multiple years with high-   frequency    observations.          The    coursework    emphasizes    the    application    of      multiple   regression    formats    and    time    series    models    to    forecast    traffic    patterns.            You      will   process      encoded      weather      data,      select      appropriate      predictors,      and      handle      data   preparation   and   analysis   through   custom   Python   modules.       This   will   enable   you   to   critically   interpret   results and   develop   a deeper   understanding of   analytical tools   and   Python   programming concepts.
Note : The   models   are NOT required to   exhibit   excellent   performance,   but they   need   to   be sensibly constructed   and   evaluated.
Key Objectives: 
1.       Decode    and    pre-process    (e.g.,    set    regular    time    intervals,    handle    missing
values, identify trends, etc.) the weather and traffic datasets   provided.    You   will   likely   not   need all of the   weather   data.
2.       Briefly explore the   data   to   demonstrate   understanding   of   its   contents   (e.g.,   statistical   reporting and a few visualisations,   maximum 5).
3.       Select    relevant    predictors   for   modelling,   justifying   your   choices   based   on   data    exploration    and      domain       knowledge.             Hint:    this    will       likely    involve   feature engineering   (e.g., to   represent cyclical   characteristics).
4.       Apply    regression   and   time   series   models   of   multiple   types   and   designs   to   predict the sum of the number of vehicles passing the two sites combined;   these   model   types   are   limited   to   those   described   in   the   module.       Design   sensible testing targets   (e.g., a chosen time   horizon,   data splits).
5.       Thoroughly    evaluate    the       performance    of      the      models      with      appropriate   metrics.    Note features of   particular   importance   in   prediction.
6.       Compare   the    above    models   to   additional   implementations   that   include   a   representation of the Day Type to explore the   effect   of   its   inclusion.
7.       Present findings with   textual,   tabular,   and   visual   code   outputs.
8.       Explain          and       justify       the       chosen          methodologies       and          results       through   markdown annotations   in aJupyter   Notebook, ensuring you tell a   coherent   story about the   process of your   analysis.
Technical Code Requirements: 
1.       The   submitted   notebook   will   have minimal amounts   of   code   necessary   to   execute the   analysis.
2.       Analysis    code    will      reside      in    self-designed      external modules or      package   directory to   promote   exploration   of   code   reusability   and   modularity.      Only   the   code   necessary to   operate the   module   code   and   display   results   will   be   shown   in the   notebook.
a.         In terms of code, an exemplary submission   might import your coded   module(s)    and      execute       individual    functions to       load,    clean,      and prepare          the data,          display          statistics             and          explanatory          data   visualisations,   engineer   features,   select    predictors,    specify    model   parameters, train   models,   and   display   model   performance   results. 
3.       Modules,       classes,       methods,       and       functions      will       include      complete       and   explanatory   docstrings.    The   existence   of these   should   be demonstrated at   least once within the   notebook via   use of the   help()   function.
4.       Code      should       be    commented      to       enhance    code       readability      and    explain   complex   logic or   important steps.
5.       Code    should    contain    at   least   3    instances   of   formal   error   handling;   many   specific applications are   possible and acceptable   (e.g., try-except   blocks   for   data   loading   or   model fitting errors).
Written Requirements : 
1.       Organise the   notebook   into clearly   defined   and   logically   ordered   sections.
2.       Provide    any      necessary      instructions    for      setting      up      the      environment      and   dependencies,   possibly   including   a   basic   requirements file.
3.       Provide    a    description    of   your   external    module/package   organisation    and   how their elements   relate to the   larger   analysis.
4.       Explain    where    and    why    formal    error    handling    has    been    incorporated    to   enhance your code’s   robustness.
5.       Before execution   of   code   in   a   notebook   cell,   include   a   statement   describing   its    purpose    and    intent.          This    may      also      include    justifications    for    chosen   methodologies, where applicable.
6.       After   execution   of   code   in   a   notebook   cell,   describe   its   outputs   and   discuss   their   implications for your analysis.
7.       Following any   series   of   related   actions   (e.g.,   execution   of   multiple   models),   provide a critical comparison of   their features,   strengths,   and   weaknesses.
8.       Conclude   the    notebook   with    a    recap   of   the   key   insights   gained   from   the   analyses,   highlighting   the   effectiveness   of   different   modelling   approaches,   acknowledging       any       data       or          methodological       limitations,       and       suggest   potential future   improvements.



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
