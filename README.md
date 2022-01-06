# How To Get the API MyAnimeList

1. Go to dashboard myAnimeList, click <code>API</code>

![Step 1](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/step%201.png "Step 1")

> Notes:
> - You can request up to 3 IDs.
> - We will occasionally review applications that use the API and their services.
> - If your application does not comply with Terms of Use of the API, we will terminate the application's access.
> - Please make sure the email address on your account is up-to-date before creating a Client ID.
> - For questions, bug reports, and general discussion about the API, please join us at the [MAL API Club](https://myanimelist.net/clubs.php?cid=13727 "MAL API Club").

2. Scroll and click <code>Create ID</code>

![Step 2](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/step%202.png "Step 2")

3. Fill all forms about what your project, read the API License and Developer Agreement and accept it, and <code>Submit</code>

> _For Section **App Logo URL, Privacy Policy URL, Terms of Use URL**_ is opsional

![Step 3](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/step%203.png "Step 3")

4. Return to list of your API. If there is a PUBLISHED message, then your API can already be used

![Step 4](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/step%204.png "Step 4")

5. Click <code>Edit</code> on your API and the Section of **Client ID and Client Secret** that we will use

![Step 5](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/Step%205.png "Step 5")


> **Tools**
> - [Python](https://www.python.org/downloads/ "Download Python") (At the time this tutorial was created, the latest version is 3.10.1)
> - Code Editor, like Notepad++, VS Code, etc

6. Download the code and open <code>mal.py</code> and change <code>YOUR_CLIENT_ID</code> and <code>YOUR CLIENT_SECRET</code>

![Step 6](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/Step%201.1.png "Step 6")

7. Open CMD or PowerShell or GitBash on your computer and type <code>pip install requests</code>

![Step 7](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/step%207.png "Step 7")

And enter it. And then copy the URL

![Step 7.1](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/Step%207.1.png "Step 7.1")

8. Open your browser and paste the URL. Click <code>Allow</code>

![Step 8](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/step%207.2.png "Step 8")

9. After that you will be directed to the page that you have set in the API form. See in the URL box at your browser, copy code after <code>?code=</code>

![Step 9](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/Step%209.png "Step 9")

10. Back to CMD, and paste it. Click enter

![Step 10](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/step%209.1.png "Step 10")


> **Tools**
> - Processing API application, i use [Postman](https://www.postman.com/downloads/ "Download Postman")

11. Close your CMD and see your folder. Open the <code>token.json</code>

![Step 11](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/Step%2011.png "Step 11")

12. Open Postman and create the new Workspace. Click Workspaces at the header of application, and Create Workspace

![Step 12](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/Step%2012.png "Step 12")

13. Fill all Forms and enter
14. At the left of your Workspace, click import

![Step 14](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/Step%2014.png "Step 14")

15. Copy this code

<code>curl 'https://api.myanimelist.net/v2/anime?q=one&limit=4' \
-H 'Authorization: Bearer YOUR_TOKEN'</code>
 and change YOUR_TOKEN. Click continue and click import

![Step 15](https://github.com/nurkholiqansori/apiMyAnimeList/blob/main/img/Step%2015.png "Step 15")
