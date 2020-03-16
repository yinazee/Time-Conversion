# Time-Conversion
HackerRank Challenge - Javascript Solution

function timeConversion(s) {

    // s = 07:05:45PM

    // 1 = 13
    // 2 = 14

    // will output [ '07', '05', '45' ]
    let timeArr = s.slice(0, -2).split(":")
    
    // will output AM or PM
    let ampm = s.slice(-2)

    // FOR 12AM, it should output 00:00:00
        if (ampm === "AM" && timeArr[0] === "12") {
            timeArr[0] = "00"
        }else if (ampm === "PM") {
        //add 12 to make it military time
             timeArr[0] = (timeArr[0] % 12) + 12
        }
    }
        console.log(timeArr)
}
