# KlingAPI



<img src="https://github.com/user-attachments/assets/f70d811d-c013-4876-8dd4-b5f4b47d5b65" alt="screenshot of a video generated by Kling API" width="70%"/>
<br><br>


Kling API provides developer access to the state of the art video generation capability from the Kling model! And we are currently looking to add Kling API as part of our generative AI API offering!
If you'd like to be notified when the feature goes online, please sign up for our waitlist [here](https://piapi.ai/kling-api)!


<h2>Features</h2>
<ol>
  <li>Video Generation Based on Input Image</li>
  <li>Stunning Camera Views</li>
  <li>Video Extension Function</li>
  <li>Extended Video Length Generation</li>
  <li>Real-World Physics Simulation</li>
  <li>HTTPS POST/GET API Calls</li>
  <li>Vivid Storytelling Capabilities</li>
  <li>Aspect Ratio Control</li>

</ol>




<h2>Usage Options</h2>

<h3>Pay-as-you-go Option</h3>

<p>
To get started, go to our [Workspace](https://app.piapi.ai/) and sign up if you haven't. Once you do, you can use the API KEY obtained to make calls to the API directly!
</p>

<ul>
  <li>You wouldn't need to buy your Kling account!</li>
  <li>You don't have to manage / operate the Kling Accounts either</li>
  <li>Users would have access to all the supported features</li>
  <li>Using this service option enable rapid prototyping!</li>
</ul>

<br>

<h3>Host-your-account Option</h3>
<p>
  When you choose our Host-Your-Account service, you will be expected to buy/operate/manage your own pool of Kling account(s). You can will then be required to subscribe to PiAPI's API seat(s), and connect your Kling account(s) to the seat(s). Then by calling our API, we will route the submitted tasks to the accounts for processing and return back the results upon their completion!
</p>

<ul>
  <li>Dedicated accounts means lower wait time</li>
  <li>Able to scale by increasing the number of account-seat combinations</li>
  <li>Cost effective Service Option for developers with varying amount of tasks loads</li>
</ul>

<br>

<h3>Pricing</h3>
Please refer to our <a href="https://piapi.ai/pricing">pricing page</a> for more information. 
<br><br>


<h2>Usage Steps</h2>
<h3>Pay-as-you-go Option</h3>

<br>
<h4>Sample API Calls (using cURL)</h4>
<br>
<p>Create a video generation </p>

```
curl --location 'https://api.piapi.ai/kling/videogen' \
--header 'X-API-Key: your_api_key_here' \
--header 'Content-Type: application/json' \
--data '{
  "input": 
        {
            "prompt":"a child running freely in the park",
        }
}'
```
<p>Response</p>

```
{
    "code": 200,
    "data": {
        "task_id": "record_this_taskID"
    },
    "message": "success"
}
```
<br>
<p>Fetching for the video generated</p>

```
curl --location 'https://api.piapi.ai/kling/fetch' \
--header 'X-API-Key: your_api_key_here' \
--header 'Content-Type: application/json' \
--data '{

            "task_id": "insert_recorded_taskID_here"
        
}'
```
<br>
<p>Response - Check out our <a href="https://piapi.ai/docs/">documentation</a> for more information!</p>
<br>
