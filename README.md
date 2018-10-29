# my-katas-demo
The demo folder that demonstrates how students could save the katas they did. 
If the students do katas on multiple websites, they could organize them into folders inside this folder (CodeWars, HackerRank, LeetCode).

- The student should do **at least 3 katas a week during the lecture weeks** and **5 katas a week during the project weeks**.
- The student should thrive to **score as better score as possible** on CodeWars or any other online learning platforms and should include proudly their ranking on their resumes and LinkedIn accounts next to the link to their GitHub account.
- The student should start solving any given challenge using the **white-board approach and sudocode**.
- The student should **reiterate** their first solution and **refactor** it to the better one (meaning the one that's more time efficient, that
has cleaner code, that is possibly shorter).
- The student should **create a folder on their GitHub** account and **save their solutions**. 
- After submitting their own solution on the let's say Codewars, they should check other best-ranked solutions and try to understand why other solutions are better ranked. The student **should save both solutions** and keep them in the record so the process of preparing for job interviews would be easier since all the code resources would be saved in one spot.

## Example:
```js
// ************************************************************************************
// https://www.codewars.com/kata/array-dot-diff/train/javascript
// Your goal in this kata is to implement a difference function, which subtracts one list from another and returns the result.
// It should remove all values from list a, which are present in list b.
// array_diff([1,2],[1]) == [2]
// If a value is present in b, all of its occurrences must be removed from the other:
// array_diff([1,2,2,2,3],[2]) == [1,3]
// ************************************************************************************


//////// my solution: ////////
const array_dif = (someArr, aThing) => {
    const updArr = [];
    someArr.forEach(elem => !aThing.includes(elem) ? updArr.push(elem) : null)
    return updArr;
}

//////// the best solution: ////////
const array_diff = (a, b) => {
    return a.filter(elem => !b.includes(elem));
};
```
