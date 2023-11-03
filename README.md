# calculator
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL"
        crossorigin="anonymous"></script>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
        integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
        crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.12.9/dist/umd/popper.min.js"
        integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
        crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
        crossorigin="anonymous"></script>

<style>
    wrapper ul {
	list-style: none;
	padding: 0;
}
.wrapper ul:after {
	content: '';
	display: table;
	clear: both;
}
.wrapper ul li:nth-child(1n + 4) {
	max-height: 0;
	opacity: 0;
	transition: 0.2s ease-in;
}
.wrapper .btn-area {
	cursor: pointer;
	font-size: 10px;
	text-align: center;
	font-weight: 900;
	width: 180px;
	border-radius: 50px;
}
.wrapper .btn-area .btn2 {
	display: none;
}
.wrapper #btnBox {
	display: none;
}
.wrapper #btnBox:checked~ul li:nth-child(1n + 4) {
	max-height: 1000px;
	opacity: 1;
	transition: 0.2s ease-in;
}
.wrapper #btnBox:checked~.btn-area .btn2 {
	display: block;
}
.wrapper #btnBox:checked~.btn-area .btn1 {
	display: none;
}
/* wrapper2*/
.Completed ul {
	list-style: none;
	padding: 0;
}
.Completed ul:after {
	content: '';
	display: table;
	clear: both;
}
.Completed ul li:nth-child(1n + 4) {
	max-height: 0;
	opacity: 0;
	transition: 0.2s ease-in;
}
.Completed .btn-area-2 {
	cursor: pointer;
	font-size: 10px;
	text-align: center;
	font-weight: 900;
	width: 180px;
	border-radius: 50px;
}
.Completed .btn-area-2 .btn4 {
	display: none;
}
.Completed #btnbox {
	display: none;
}
.Completed #btnbox:checked~ul li:nth-child(1n + 4) {
	max-height: 1000px;
	opacity: 1;
	transition: 0.2s ease-in;
}
.Completed #btnbox:checked~.btn-area-2 .btn4 {
	display: block;
}
.Completed #btnbox:checked~.btn-area-2 .btn3 {
	display: none;
}








</style>


</head>

<body>
    <div id="Container1" class="flex flex-col w-1/5 mt-6">
        <div class="flex justify-center items-center bg-black text-white rounded-r-full p-1 mt-4 gap-2">
            <svg width="18" height="24" viewBox="0 0 18 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path
                    d="M10.125 14.2909H5.625C5.32663 14.2909 5.04048 14.4116 4.8295 14.6264C4.61853 14.8412 4.5 15.1326 4.5 15.4364C4.5 15.7402 4.61853 16.0315 4.8295 16.2463C5.04048 16.4612 5.32663 16.5818 5.625 16.5818H10.125C10.4234 16.5818 10.7095 16.4612 10.9205 16.2463C11.1315 16.0315 11.25 15.7402 11.25 15.4364C11.25 15.1326 11.1315 14.8412 10.9205 14.6264C10.7095 14.4116 10.4234 14.2909 10.125 14.2909ZM14.625 2.83638H13.2975C13.0654 2.16795 12.6359 1.58898 12.0679 1.17884C11.5 0.768696 10.8213 0.547464 10.125 0.545471H7.875C7.17869 0.547464 6.50002 0.768696 5.93205 1.17884C5.36408 1.58898 4.9346 2.16795 4.7025 2.83638H3.375C2.47989 2.83638 1.62145 3.19843 0.988515 3.84287C0.355579 4.48731 0 5.36136 0 6.27274V20.0182C0 20.9296 0.355579 21.8036 0.988515 22.4481C1.62145 23.0925 2.47989 23.4546 3.375 23.4546H14.625C15.5201 23.4546 16.3786 23.0925 17.0115 22.4481C17.6444 21.8036 18 20.9296 18 20.0182V6.27274C18 5.36136 17.6444 4.48731 17.0115 3.84287C16.3786 3.19843 15.5201 2.83638 14.625 2.83638ZM6.75 3.98184C6.75 3.67804 6.86853 3.38669 7.0795 3.17188C7.29048 2.95706 7.57663 2.83638 7.875 2.83638H10.125C10.4234 2.83638 10.7095 2.95706 10.9205 3.17188C11.1315 3.38669 11.25 3.67804 11.25 3.98184V5.12729H6.75V3.98184ZM15.75 20.0182C15.75 20.322 15.6315 20.6133 15.4205 20.8282C15.2095 21.043 14.9234 21.1637 14.625 21.1637H3.375C3.07663 21.1637 2.79048 21.043 2.5795 20.8282C2.36853 20.6133 2.25 20.322 2.25 20.0182V6.27274C2.25 5.96895 2.36853 5.6776 2.5795 5.46279C2.79048 5.24797 3.07663 5.12729 3.375 5.12729H4.5V6.27274C4.5 6.57654 4.61853 6.86789 4.8295 7.0827C5.04048 7.29752 5.32663 7.4182 5.625 7.4182H12.375C12.6734 7.4182 12.9595 7.29752 13.1705 7.0827C13.3815 6.86789 13.5 6.57654 13.5 6.27274V5.12729H14.625C14.9234 5.12729 15.2095 5.24797 15.4205 5.46279C15.6315 5.6776 15.75 5.96895 15.75 6.27274V20.0182ZM12.375 9.70911H5.625C5.32663 9.70911 5.04048 9.82979 4.8295 10.0446C4.61853 10.2594 4.5 10.5508 4.5 10.8546C4.5 11.1584 4.61853 11.4497 4.8295 11.6645C5.04048 11.8793 5.32663 12 5.625 12H12.375C12.6734 12 12.9595 11.8793 13.1705 11.6645C13.3815 11.4497 13.5 11.1584 13.5 10.8546C13.5 10.5508 13.3815 10.2594 13.1705 10.0446C12.9595 9.82979 12.6734 9.70911 12.375 9.70911Z"
                    fill="white" />
            </svg>


            <button id="task" class="bg-black  text-white rounded-r-full p-2">Task</button>
        </div>

        <div class="flex justify-center items-center bg-black text-white rounded-r-full p-2 mt-4 gap-2">
            <svg width="18" height="24" viewBox="0 0 18 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path
                    d="M9 0.545471C6.61305 0.545471 4.32387 1.51092 2.63604 3.22943C0.948212 4.94794 0 7.27874 0 9.70908C0 15.8945 7.93125 22.8818 8.26875 23.1796C8.47252 23.357 8.73185 23.4546 9 23.4546C9.26815 23.4546 9.52748 23.357 9.73125 23.1796C10.125 22.8818 18 15.8945 18 9.70908C18 7.27874 17.0518 4.94794 15.364 3.22943C13.6761 1.51092 11.3869 0.545471 9 0.545471ZM9 20.7627C6.60375 18.4718 2.25 13.5349 2.25 9.70908C2.25 7.88632 2.96116 6.13822 4.22703 4.84934C5.4929 3.56046 7.20979 2.83637 9 2.83637C10.7902 2.83637 12.5071 3.56046 13.773 4.84934C15.0388 6.13822 15.75 7.88632 15.75 9.70908C15.75 13.5349 11.3962 18.4832 9 20.7627ZM9 5.12727C8.10998 5.12727 7.23996 5.39599 6.49993 5.89945C5.75991 6.4029 5.18314 7.11848 4.84254 7.9557C4.50195 8.79291 4.41283 9.71416 4.58647 10.6029C4.7601 11.4917 5.18868 12.3081 5.81802 12.9489C6.44736 13.5897 7.24918 14.0261 8.12209 14.2028C8.99501 14.3796 9.89981 14.2889 10.7221 13.9421C11.5443 13.5953 12.2471 13.0081 12.7416 12.2546C13.2361 11.5011 13.5 10.6153 13.5 9.70908C13.5 8.49391 13.0259 7.32851 12.182 6.46925C11.3381 5.61 10.1935 5.12727 9 5.12727ZM9 12C8.55499 12 8.11998 11.8656 7.74997 11.6139C7.37996 11.3622 7.09157 11.0044 6.92127 10.5858C6.75097 10.1672 6.70642 9.70654 6.79323 9.26215C6.88005 8.81775 7.09434 8.40955 7.40901 8.08917C7.72368 7.76878 8.12459 7.55059 8.56105 7.46219C8.9975 7.3738 9.4499 7.41917 9.86104 7.59256C10.2722 7.76595 10.6236 8.05958 10.8708 8.43632C11.118 8.81306 11.25 9.25598 11.25 9.70908C11.25 10.3167 11.0129 10.8994 10.591 11.329C10.169 11.7586 9.59674 12 9 12Z"
                    fill="white" />
            </svg>
            <button id="location"><a style="text-decoration: none;" href="Location.html">location</a></button>

        </div>
        <div id="butten" class="flex absolute bottom-10 pl-10 bg-white text-white rounded-r-full p-1  gap-2">
            <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path
                    d="M7 19H3C2.46957 19 1.96086 18.7893 1.58579 18.4142C1.21071 18.0391 1 17.5304 1 17V3C1 2.46957 1.21071 1.96086 1.58579 1.58579C1.96086 1.21071 2.46957 1 3 1H7"
                    stroke="black" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
                <path d="M14 15L19 10L14 5" stroke="black" stroke-width="2" stroke-linecap="round"
                    stroke-linejoin="round" />
                <path d="M19 10H7" stroke="black" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
            </svg>

            <button id="button3" class="text-black"><a style="text-decoration: none;" href="login.html">Log
                    Out</a></button>

        </div>

    </div>

    <div id="Container2" class=" ... w-96 h-5/6 absolute top-10 left-96 space-y-4">
        <button id="addtask" class="font-medium" data-toggle="modal" data-target="#exampleModalCenter">+ Add New
            Task</button>
 <input type="text" id="simple-search" onkeyup="abc()" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-80 pl-10 p-2.5  dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="Search branch name..." required>

            <!-- <button type="submit" class="p-2.5 ml-2 text-sm font-medium text-white bg-blue-700 rounded-lg border border-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
                <svg class="w-4 h-4" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 20">
                    <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m19 19-4-4m0-7A7 7 0 1 1 1 8a7 7 0 0 1 14 0Z"/>
                </svg>
                <span class="sr-only">Search</span>
            </button> -->

        <h5 class="font-medium">Incomplete</h5>
        <div class="wrapper">
            <input type="checkbox" id="btnBox">
            <ul class="list " id="contentList">
                    
            </ul>
            <label class="btn-area" for="btnBox">
                <span class="btn1">LOAD MORE</span>
                 <span class="btn2">LOAD LESS</span></label>
        </div>
        <div class="complete-task">
            <h5 class="py-3"><b>Completed</b></h5>
           
                        <div class="Completed">
                            <input type="checkbox" id="btnbox">
            <ul class="list " id="completed">
                    
                    </ul>
                    <label class="btn-area-2" for="btnbox">
                        <span class="btn3">LOAD MORE</span>
                         <span class="btn4">LOAD LESS</span></label>
                    
        </div>
       

        </div>
    
        <!-- </div>
    <div class="col">
    </div> -->
</div>
</div>

    <!-- Button trigger modal -->

    <!-- Modal -->
    <div class="modal fade" id="exampleModalCenter" tabindex="-1" role="dialog"
        aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered" role="document">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title font-medium" id="exampleModalLongTitle">New Task</h5>
                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                        <!-- <span aria-hidden="true">&times;</span> -->
                    </button>
                </div>
                <div class="modal-body">
                    <div class="container">
                        <div class="row">
                            <div class="mx-auto py-4 space-y-4 newtask">
                                <input id="taskInput" type="text" class="icon py-2 mx-5 px-5" placeholder="Summary">
                                <input type="text" class="dp mx-5 px-5 py-3" value placeholder="Description">
                                <input id="date" type="date" class="date mx-5 px-5" placeholder="Due Date">
                                <div class="d-grid gap-2 d-flex flex-col items-center justify-content-center">
                                    <button id="add"
                                        class="flex items-center justify-center w-60 rounded-full font-medium bg-black text-white px-2 py-2"
                                        type="button">Save</button>

                                    <button class="btn btn-primary w-60 rounded-full border-none Class
                            Properties
                            transition-colors hover:bg-white font-medium text-black" type="button"
                                        data-dismiss="modal">Cancel</button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>


    <script type="text/javascript">






    let taskInput = document.getElementById('taskInput');
    let taskList = document.getElementById('contentList');
    let addBtn = document.getElementById('add');
    let completed = document.getElementById('completed');
    let date = document.getElementById("date")
       

        function getNewTask() {

            let newTask = taskInput.value;
             let newdate = date.value
            // console.log(newTask)
            taskList.innerHTML += `

            <li>
                    <input class="mx-5 text-dark" type="checkbox" id="Todo" name="todolist" value="task-1" onchange="completeTask(this)">
                    <label for="todolist">${newTask} ${newdate} </label>
                    
            </li>

            `
            saveData()
        }

        addBtn.addEventListener('click', getNewTask);

        function completeTask(checkbox) {

            if (checkbox.checked) {
                completed.append(checkbox.parentElement);
            } else {
                taskList.append(checkbox.parentElement);
            }
            saveData()
        }

        //DAta Save Function
        function saveData() {
            localStorage.setItem('contentList', taskList.innerHTML);
            localStorage.setItem('completed', completed.innerHTML);
        }
        //Data Get Function
        function showTask() {
            let savedIncompleteTasks = localStorage.getItem('contentList');
            let savedCompletedTasks = localStorage.getItem('completed');
            if (savedIncompleteTasks) {
                taskList.innerHTML = savedIncompleteTasks;
            }
            if (savedCompletedTasks) {
                completed.innerHTML = savedCompletedTasks;
            }
        }
        showTask()

        




    </script>

</body>

</html>
