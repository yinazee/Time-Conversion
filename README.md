# Time-Conversion
HackerRank Challenge - Javascript Solution

function timeConversion(s) {

    // s = 07:05:45PM

    // 1 = 13
    // 2 = 14
    // 3 = 15
    // 4 = 16
    // 5 = 17
    // 6 = 18
    // 7 = 19
    // 8 = 20
    // 9 = 21


    let hour = s.slice(0, -2).split(":")
    let ampm = s.slice(-2)


    if (ampm === "AM") {

        if (hour[0] === 0) {
            hour = hour[1] + 12
            console.log(hour[1])
        }
           
    
    }

 
}
