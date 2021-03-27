<template>
    <div>
        <div class="page-title">
            <div class="page-left">Danh sách nhân viên</div>
            <div class="page-right">
                <button id="btn-add" class="btn-default add-customer-btn">Thêm nhân viên</button>
            </div>
        </div>
        <div class="toolbar">
            <input type="text" class="input-search" placeholder="Tìm kiếm theo mã, tên nhân viên" />
            <button class="btn-refresh"></button>
            <button class="btn-delete">Xóa</button>
        </div>
    </div>
</template>

<style scoped>
.page-title{height: 40px;display: flex;align-items: center;}

.page-title .page-right{
    position:  absolute;
    right: 24px;
}

.page-title .page-left{
    font-size: 24px;
    font-weight:bold;
}

.toolbar{
    margin-top: 16px;
    display: flex;
    width: 100%;
    align-items: center;
    height: 42px;
    /* background-color: #ff0000; */
}
</style>