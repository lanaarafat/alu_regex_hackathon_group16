// Regular expression for Twitter usernames
const twitterUsernameRegex = /@(\w+)/;

// Regular expression for ISBN numbers
const isbnRegex = /ISBN (\d{3}-\d-\d{3}-\d{5}-\d)/;

// Regular expression for jokes
const jokeRegex = /Why did the (.+)\? Because(.+)/;

// Regular expression for weirdly formatted dates
const weirdDateFormatRegex = /\b(0[1-9]|[1-2][0-9]|3[01])-(?:Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)-(19|20)\d{2}\b/;

// Test data
const testData = [
  "@username",
  "ISBN 123-4-567-89012-3",
  "Why did the chicken cross the road? Because it wanted to get to the other side!",
  "25-May-2023",
];

// Match Twitter usernames
console.log("Twitter usernames:");
testData.forEach((data) => {
  const match = data.match(twitterUsernameRegex);
  if (match) {
    console.log(match[1]);
  }
});

// Match ISBN numbers
console.log("\nISBN numbers:");
testData.forEach((data) => {
  const match = data.match(isbnRegex);
  if (match) {
    console.log(match[1]);
  }
});

// Match jokes
console.log("\nJokes:");
testData.forEach((data) => {
  const match = data.match(jokeRegex);
  if (match) {
    console.log(`Q: ${match[1]}`);
    console.log(`A: ${match[2]}`);
  }
});

// Match weirdly formatted dates
console.log("\nWeirdly formatted dates:");
testData.forEach((data) => {
  const match = data.match(weirdDateFormatRegex);
  if (match) {
    const day = match[1];
    const month = match[2];
    const year = match[3];
    console.log(`${day}-${month}-${year}`);
  }
});

