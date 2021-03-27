<template>
    <div id="header">
        <div class="header-title">
            <select class="header-select" name="" id="">
                <option value="">Nhà hàng biển Đông</option>
                <option value="">Nhà hàng Hải Dương</option>
                <option value="">Nhà hàng Đội Cấn</option>
                <option value="">Nhà hàng Cầu Giấy</option>
            </select>
        </div>
        <div class="header-user">
            <img src="../../assets/img/default-avatar.jpg" alt="avatar" class="user-avatar">
            <div class="user-name">
                <span>Ngọc Dũng</span>
                <i class="fas fa-ellipsis-h header-option"></i>
            </div>
        </div>
    </div>
</template>

<style scoped>
#header {
    border: 1px solid #dedede;
    position: absolute;
    left:200px;
    right:0;
    height: 60px;
    top:0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    /* background-color: #4cff00; */
}

.header-select {
    border-color: transparent;
    font-size: 1.4rem;
    font-weight: bold;
    margin-left: 30px;
    outline: none;
}

.header-user {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-right: 20px;
}

.user-avatar {
    width: 25px;
    height:25px;
    border-radius:50%;
}

.user-name > span{
    font-size: 1.4rem;
    margin: auto 5px;
}
</style>