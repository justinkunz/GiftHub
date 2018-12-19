# GiftHub
GiftHub matches people struggling to find gifts with self proclaimed gifting experts. Annonymously submit a request
for help, or lend a hand to someone in need by helping them find the perfect present for the special someone
in their life. This free, anonymous service requires no account registration and can be used for any occasion.
Get gifting today! _try a live demo at http://

## How It Works
1. Users needing help finding gifts fill out a form under the Ask for Help section of the site
2. Self Proclaimed Gift Experts are matched with your request under the Help Someone section of the site. 
3. An email is sent the user that requested help that includes a link and message from the Gift Expert that responded to the request

## The Chrome Extension
GiftHub also includes a chrome extension! This chrome extension allows Gift Experts to pass in links as gift suggestions. To install an unpacked chrome extension:
    * Clone this repo to your local machine
    * Vist Chrome://extensions in Google Chrome
    * Toggle Developer Mode
    * Click Load Unpacked Extension
    * Navigate to the cloned repo, and find the __chrome__ folder

## Link Tracking
The links embeeded to response emails are tracked for analytic purposes. When a user clicks the link to view the suggested gift, they are sent to GiftHub, where their click is logged in the links table of the database. This is to count the number of times the gift requester will view the requested gift

## Link Conversion & Monetization
A function is included in the __apiroutes.js__ file to convert validate & and convert suggested __Amazon__ links. This is the monetization method of this site. When a user submits a gift suggestion, a function on the backend will determine if the link the user passed in was from Amazon. If it was, it will convert it to an affiliate link, so if the requestee buys the item, Amazon will pay a commission. This process does not change the suggested product, just the link that the requestee will see. 
_for example: https://www.amazon.com/dp/B01DFKC2SO/ref=ods_gw_d_stage5_bis_xpl1?pf_rd_p=05d51bae-1820-4c75-8921-c2a1fd4030de&pf_rd_r=P8E7H98D63R7JPVG4AP4 becomes https://www.amazon.com/dp/B01DFKC2SO/?tag=gifthelp03-20_

## Try it Out!

