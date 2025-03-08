# Web-Client-Development

function rectangleArea(length, width) {
    return length * width;
}
console.log(rectangleArea(5, 3));

function circleProperties(radius) {
    let diameter = 2 * radius;
    let circumference = 2 * Math.PI * radius;
    let area = Math.PI * radius * radius;
    return {
        diameter,
        circumference: Number(circumference.toFixed(4)),
        area: Number(area.toFixed(3))
    };
}
console.log(circleProperties(5)); 

function thirdAngle(a, b) {
    return 180 - (a + b);
}
console.log(thirdAngle(80, 65)); 

function dateDifference(date1, date2) {
    let d1 = new Date(date1);
    let d2 = new Date(date2);
    let difference = Math.abs(d2 - d1) / (1000 * 60 * 60 * 24);
    return difference;
}
console.log(dateDifference("2024-03-19", "2024-03-21")); 

function nameInitials(name) {
    return name.split(' ').map(word => word[0].toUpperCase()).join('');
}
console.log(nameInitials("John Doe")); 
