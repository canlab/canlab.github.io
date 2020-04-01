CANlabCore README

Steps to publish a new walkthrough or modified one:

1. Modify/create Matlab script for walkthrough in canlab_help_examples/example_help_files

2. Run canlab_help_publish.m with your script to create html in CANlab_help_examples/published_html/

3. Copy html folder to canlab.github.io repository, in "_pages" folder. You must first clone the repo on your local computer. Then you can edit pages/files and commit + push using github the same way you would any repository.  

4. Modify markdown page in canlab.github.io to link to the example walkthrough (if new or renamed)

5. Commit to canlab.github.io and push repo to Master. When you do this, it will attempt to build automatically on the server.

6. Wait a bit for it to build on the github server, and check that the walkthrough is linked correctly/accessible, and looks as intended. There is a site to check the build status.
