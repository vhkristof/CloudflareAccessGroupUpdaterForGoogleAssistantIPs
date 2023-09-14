#testing
# CloudflareAccessGroupUpdaterForGoogleAssistantIPs
Script for automatically updating a [CloudFlare Access group](https://developers.cloudflare.com/cloudflare-one/identity/users/groups/) to include all the IP addresses used by Google Assistant.

## CloudFlare setup
1. [Get your account ID](https://developers.cloudflare.com/fundamentals/get-started/basic-tasks/find-account-and-zone-ids/)
2. [Create an API token with following permissions](https://developers.cloudflare.com/fundamentals/api/get-started/create-token/):
    * Access: Organizations, Identity Providers, and Groups: Edit
    * Access: Organizations, Identity Providers, and Groups: Read
3. [Create an access group in your Zero Trust environment](https://developers.cloudflare.com/cloudflare-one/identity/users/groups/)

## Script setup
    git clone https://github.com/vhkristof/CloudflareAccessGroupUpdaterForGoogleAssistantIPs
    pip install -r requirements.txt
    python script.py --account <id from step 1> --token <id from step 2> --group <id from step 3>
