1.build resume using json
const resume={
  "name": "Madhavakumaran",
  "email": "kumaranmadhava9@gmail.com",
  "phone": "6379028897",
  "address": "pondicherry",
  "education": [
    {
      "degree": "Bachelor of Technology",
      "university": "pondicherry university",
      "year": "20"
    },
    {
      "degree": "High School Diploma",
      "university": "ABC High School",
      "year": "2011"
    }
  ],
  "skills": [
    "JavaScript",
    "Python",
    "HTML/CSS",
    "SQL"
  ]
}
console.log(resume)

for loop for in loop for each


const resume = {
  "name": "Madhavakumaran",
  "email": "kumaranmadhava9@gmail.com",
  "phone": "6379028897",
  "address": "Pondicherry",
  "education": [
    {
      "degree": "Bachelor of Technology",
      "university": "Pondicherry University",
      "year": "2022"
    },
    {
      "degree": "High School Diploma",
      "university": "ABC High School",
      "year": "2011"
    }
  ],
  "skills": [
    "JavaScript",
    "Python",
    "HTML/CSS",
    "SQL"
  ]
};

// Using "'for"' loop
console.log("Using 'for' loop:");
for (let key in resume) {
  console.log(key + ": " + resume[key]);
}

// Using '"for...in'" loop
console.log("\nUsing 'for...in' loop:");
for (let key in resume) {
  if (resume.hasOwnProperty(key)) {
    console.log(key + ": " + resume[key]);
  }
}

// Using '"forEach'" loop on education array
console.log("\nUsing 'forEach' loop on education array:");
resume.education.forEach((edu) => {
  console.log("Degree: " + edu.degree);
  console.log("University: " + edu.university);
  console.log("Year: " + edu.year);
});

// Using 'f"or...of'" loop on skills array
console.log("\nUsing 'for...of' loop on skills array:");
for (let skill of resume.skills) {
  console.log(skill);
}
