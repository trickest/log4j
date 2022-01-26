# Trickest Log4j

## Short description

Apache Log4j2 versions 2.0-beta7 through 2.17.0 (excluding security fix releases 2.3.2 and 2.12.4) are vulnerable to a remote code execution (RCE). 

## Motivation

After a huge number of bypass payloads, we decided it is the right time to automate everything through [Trickest](https://trickest.com) workflow and just add new vectors to this repository which would alter the workflow and potentially bypass current fixes.

### Different techniques

Constantly updated

You can checkout [issues](https://github.com/trickest/log4j/issues) for our current ideas that will be implemented in the future versions of the workflow. [README.md](http://README.md) will be updated accordingly.

Scalability

Workflow is currently capable of getting the list of hostnames executing the workflow explained in TB;DZ. Through issues, it will be constantly updated as well as all the payloads used in inside of the workflow.

Customization

Workflow is entirely customizable to support different range of use-cases:
 * By changing the payloads in ```payloads``` folder it will pick up new ones and execute workflow.
 * By adding new nuclei templates in ```custom``` folder will alter the [nuclei](https://github.com/projectdiscovery/nuclei) execution.

- Process
    - Workflow screenshot
    - TB; DZ explanation
- Lessons Learned
    - 
- Resources (give credit to original authors)
    - tools
        - [cent](https://github.com/xm1k3/cent)
        - [cent-yaml](https://github.com/trickest/log4j/issues)
        - [nuclei](https://github.com/projectdiscovery/nuclei)
        - [unfurl](https://github.com/tomnomnom/unfurl)
        - [thchydra](https://github.com/vanhauser-thc/thc-hydra)
    - payloads
        - payload - twitter/github links
    - nuclei-templates
        - template-id - https://github.com/author

# Directory Structure

- **payloads**
    - manual.txt # files that are added to the repository manually by editing the workflow, or by committing to this repository
    - null-bytes.txt
    - tab.txt
    - new-line.txt
    - all.txt
- **nuclei-templates**
    - custom
    - community
- services.txt
- example-report.txt
- **README.md**