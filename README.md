# Class-vs.-Instance
HackerRank Challenges
function Person(initialAge) {
  if (initialAge >= 0) {
    this.age = initialAge;
  } else {
    process.stdout.write("Age is not valid, setting age to 0.\n")
    this.age = 0;
  }

  this.amIOld=function(){
    if (this.age < 13) {
      process.stdout.write("You are young.\n");
    }
    else if (this.age < 18) {
      process.stdout.write("You are a teenager.\n");
    }
    else {
      process.stdout.write("You are old.\n");
    }

  };
  this.yearPasses=function(){
    this.age++;
  };
}
