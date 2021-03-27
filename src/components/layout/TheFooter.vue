<template>
    <div class="footer">
        <div class="number-customer">
            <p>Hiển thị 1-10/1000 khách hàng</p>
        </div>
        <div class="switch-page">
            <img src="../../assets/icon/btn-firstpage.svg" alt="first-page-btn" class="first-page-btn">
            <img src="../../assets/icon/btn-prev-page.svg" alt="prev-page-btn" class="first-page-btn">
            <div class="page-index" style="background-color: #019160;">
                <span>1</span>
            </div>
            <div class="page-index">
                <span>2</span>
            </div>
            <div class="page-index">
                <span>3</span>
            </div>
            <div class="page-index">
                <span>4</span>
            </div>
            <img src="../../assets/icon/btn-next-page.svg" alt="next-page-btn" class="first-page-btn">
            <img src="../../assets/icon/btn-lastpage.svg" alt="last-page-btn" class="first-page-btn">

        </div>
        <div class="number-customer-in-page">
            <p>10 khách hàng/trang</p>
        </div>
    </div>
</template>

<style scoped>
.footer{
    position: absolute;
    bottom:0;
    height: 60px;
    left: 24px;
    right: 24px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-top: 4px solid #727475;
}

.footer p{
    font-size: 1rem;
}

.switch-page {
    display: flex;
}

.switch-page img{
    cursor: pointer;
}

.page-index {
    display: flex;
    width: 25px;
    height:25px;
    border-radius: 50%;
    border: 1px solid #ccc;
    margin-left: 3px;
    margin-right: 3px;
    cursor: pointer;
}

.page-index:hover {
    background-color: #dedede;
}

.page-index span {
    margin: auto;
    font-size: 1.1rem;
}
</style>