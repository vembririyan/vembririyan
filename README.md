Hello, My name is Vembri Riyan, I'm a Mid Fullstack Developer :man_technologist:

I have experience in several programming languages like Java, Kotlin, PHP, JS, C#

And have experience in several frameworks like Bootstrap, Tailwind CSS, Node Js, Codeigniter,Laravel, React JS, React Native, Flutter

📫 My Contact \
E-mail   : vembrivrd@gmail.com\
Linkedin : https://www.linkedin.com/in/vembririyan/ \
Discord  : vembri_riyan

function isTimeLimit(current_date,from_swap_date,to_swap_date){
	const currentTime = new Date();
	const targetTime = new Date();
	targetTime.setHours(17, 51, 0);
	if(convertToDayofYear(to_swap_date) == convertToDayofYear(current_date)){
		return currentTime <= targetTime ? true : false;
	}else if(convertToDayofYear(from_swap_date) == convertToDayofYear(current_date)){
		return currentTime <= targetTime ? true : false;
	}
	return false;
}
function isToSwapDateMoreThanCurrentDate(current_date,from_swap_date,to_swap_date) {
	return (convertToDayofYear(to_swap_date) > convertToDayofYear(current_date)) || (convertToDayofYear(from_swap_date) > convertToDayofYear(current_date)) || isTimeLimit(current_date,from_swap_date,to_swap_date) ? true :false
}
