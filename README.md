# EmailScrapers


## # How to use this tool

1. Go to the link www.linkedin.com/company/{company_name}/people
2. Open dev tools - console
3. Input this javascript code to get the users, you need to scroll down and hit more users so all populate.
4. This does not work if it's a school, haven't figured it out yet.

    const profileTitles = document.querySelectorAll('.org-people-profile-card__profile-title');
    let textList = '';
    for (let i = 0; i < profileTitles.length; i++) {
    if (profileTitles[i].innerText === "LinkedIn Member") {
       continue;
    }
    textList += profileTitles[i].innerText + '\n';
    }
    console.log(textList);
