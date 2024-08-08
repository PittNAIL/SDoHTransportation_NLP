# SDoHTransportation_NLP
A rule-based NLP algorithm to identify transportation needs from clinical notes using the OHNLP MedTagger framework.

## Definition of Transportation Needs
| Transportation Terms | Transportation Need Terms                                                                                                                                                             |
|----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| transportation, ride, driv(e|ing) | work on, option(s), issue(s), due to, assist(ance)?, access, adequate, discuss(ed|es|ing), (un)?able, accommodation, support, agree(s)?, appl(y|ies), arrang(ed|es|ing)?, need(s), blam(e|sing)?, find(s|ing), connect(ing|ed)?, could(n't| not), did(n't|not), difficult(y|ies)?, get(ting)?, help, does(n't| not), lack(s|ing)?, easier, EMS, investigate, us(es|ing), depend(s|ing)?, organiz(es|ing), coordination, possible, resources, limit(s|ations)?, convenience, trouble(s)?, secur(e|es|ing), concern(s)?, regarding, reli(es|able|ant), time allowance, problem(s)?, challeng(es|ing), purpose(s)?, offer(s|ed), provid(es|ed|ing) |


## Getting Started with OHNLP Toolkit

### Installation and Use of MedTagger
#### Video demo: https://vimeo.com/392331446

1. Download the latest release from https://github.com/OHNLP/MedTagger/releases
2. Extract the zip file
3. Modify the `INPUTDIR`, `OUTPUTDIR`, and `RULEDIR` variables in `run_medtagger_win.bat` or `run_medtagger_unix_mac.sh`, as appropriate
    - `INPUT_DIR`: full directory path of input folder 
    - `OUTPUT_DIR`: full directory path of output folder
    - `RULES_DIR`: full directory path of 'Rule' folder
    
    Example for Mac:
    ```
    INPUTDIR="$YOUR_INPUT_DIRECTORY"
    OUTPUTDIR="$YOUR_OUTPUT_DIRECTORY"
    RULEDIR="$YOUR_MEDTAGGER_HOME/medtaggerieresources/covid19"
    ```
    
    Example for Windows:
    ```
    INPUTDIR="C:\$YOUR_INPUT_DIRECTORY\input"
    OUTPUTDIR="C:\$YOUR_OUTPUT_DIRECTORY\output"
    RULEDIR="C:\YOUR_MEDTAGGER_HOME\medtaggerieresources\covid19"
    ```
    
4. Run the batch file

    Mac/linux: 
    ```
    run_medtagger_unix_mac.sh
    ```
    
    Windows: 
    
    ```
    run_medtagger_win.bat
    ```
