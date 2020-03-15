# Time-Conversion
HackerRank Challenge - Javascript Solution

function timeConversion(s) {

    // s = 07:05:45PM

    // 1 = 13
    // 2 = 14

    // will output [ '07', '05', '45' ]
    let hour = s.slice(0, -2).split(":")
    // will output AM or PM
    let ampm = s.slice(-2)

    // FOR 12AM, it should output 00:00:00
    if (ampm === "AM") {

        if (hour[0] === 0) {
            hour = hour[1] + 12
            console.log(hour[1])
        }
           
    
    }

 
}
