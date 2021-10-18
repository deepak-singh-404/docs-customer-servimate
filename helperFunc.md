========================
VALID MOBILE NUMBER
-------------------
const isValidPhoneNumber = (phoneNumber) => {
    let tempNumber = phoneNumber.slice(0, 3)
    if (tempNumber !== "+91") {
        return false
    }
    let number = phoneNumber.slice(3, 13)
    let regx = /^[6-9]\d{9}$/
    return regx.test(number) ? true : false
}


=======================

