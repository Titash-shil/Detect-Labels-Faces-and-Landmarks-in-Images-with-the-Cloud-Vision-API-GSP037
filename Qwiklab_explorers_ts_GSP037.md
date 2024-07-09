# Detect Labels, Faces, and Landmarks in Images with the Cloud Vision API || [GSP037](https://www.cloudskillsboost.google/focuses/1841?parent=catalog) ||

# # Like, comment, share & Don't forget to subscribe [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN) 👍😄🤝

### Run the following Commands in CloudShell
```
#----------------------------------------------------start--------------------------------------------------#

echo "${YELLOW}${BOLD}Starting${RESET}" "${GREEN}${BOLD}Execution${RESET}"

gcloud alpha services api-keys create --display-name="awesome" 

KEY_NAME=$(gcloud alpha services api-keys list --format="value(name)" --filter "displayName=awesome")

export API_KEY=$(gcloud alpha services api-keys get-key-string $KEY_NAME --format="value(keyString)")

export PROJECT_ID=$(gcloud config list --format 'value(core.project)')

gsutil mb gs://$PROJECT_ID

curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/main/Detect%20Labels%2C%20Faces%2C%20and%20Landmarks%20in%20Images%20with%20the%20Cloud%20Vision%20API/city.png

curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/main/Detect%20Labels%2C%20Faces%2C%20and%20Landmarks%20in%20Images%20with%20the%20Cloud%20Vision%20API/donuts.png

curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/main/Detect%20Labels%2C%20Faces%2C%20and%20Landmarks%20in%20Images%20with%20the%20Cloud%20Vision%20API/selfie.png

gsutil cp donuts.png gs://$PROJECT_ID

gsutil cp selfie.png gs://$PROJECT_ID

gsutil cp city.png gs://$PROJECT_ID

gsutil acl ch -u AllUsers:R gs://$PROJECT_ID/donuts.png

gsutil acl ch -u AllUsers:R gs://$PROJECT_ID/selfie.png

gsutil acl ch -u AllUsers:R gs://$PROJECT_ID/city.png

echo "${RED}${BOLD}Congratulations${RESET}" "${WHITE}${BOLD}for${RESET}" "${GREEN}${BOLD}Completing the Lab !!!${RESET}"

#-----------------------------------------------------end----------------------------------------------------------#
```
# Congratulations ..!!🎉  You completed the lab shortly..😃💯

# *Well done..!* 👏

# Thank you for visiting.... :) 🗯️

# [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN) 
