<template>
    <div class="dialog" v-show="isOpen">
        <div class="model"></div>
        <div id="dialog-content" class="dialog-content">
            <div class="dialog-header">
                <div class="dialog-title">THÔNG TIN KHÁCH HÀNG</div>
                <div @click="closeDialog" id="btn-close" class="dialog-close-button">&#x2715;</div>
            </div>
            <div class="dialog-body">
                <div class="section-top">
                    <div class="user-image">
                        <img src="../../assets/img/default-avatar.jpg" alt="avatar">
                        <p>Vui lòng chọn ảnh có địng dạng <b>.jpg, .jpeg, .png, .gif</b></p>
                    </div>
                    <div class="user-id-and-dob">
                        <label for="">Mã khách hàng(<span style="color: red">*</span>)</label>
                        <input id="txtCustomerCode" type="text" class="user-id" required>
                        <label for="">Mã thẻ thành viên</label>
                        <input type="text" class="user-id-member-card">
                        <label for="">Ngày sinh</label>
                        <input id="txtDob" type="text" class="user-dob" placeholder="mm/dd/yyyy">
                    </div>
                    <div class="user-name-and-gender">
                        <label for="">Họ và tên(<span style="color: red">*</span>)</label>
                        <input id="txtCustomerFullName" type="text" class="user-id" required>
                        <label for="">Nhóm khách hàng</label>
                        <select name="" class="customer-select">
                            <option value=""></option>
                            <option value="VIP">VIP</option>
                            <option value="MISA">Nhóm khách hàng MISA</option>
                            <option value="NOR">Khách hàng thường</option>
                        </select>
                        <label for="">Giới tính</label>
                        <div class="gender-choices">
                            <input type="radio" id="male" name="gender" value="1">
                            <label for="male">Nam</label>
                            <input type="radio" id="female" name="gender" value="0">
                            <label for="female">Nữ</label>
                            <input type="radio" id="other" name="gender" value="2">
                            <label for="other">Khác</label>
                        </div>
                    </div>
                </div>
                <div class="section-bottom">
                    <div class="user-email-and-company">
                        <label for="">Email</label>
                        <input id="txtEmail" type="text" class="user-email" placeholder="example@example.com">
                        <label for="">Tên công ty</label>
                        <input type="text" class="user-company">
                    </div>
                    <div class="user-phone-and-tax">
                        <label for="">Số điện thoại</label>
                        <input id="txtPhoneNumber" type="text" class="user-email" >
                        <label for="">Mã số thuế</label>
                        <input type="text" class="user-company-tax" placeholder="Mã số thuế của công ty">
                    </div>
                </div>
                <div class="user-address">
                    <label for="">Địa chỉ</label><br>
                    <input type="text" class="user-address-input" >
                </div>
                <div class="dialog-footer">
                    <button class="btn-default cancel-btn">
                        Hủy
                    </button>
                    <button id="btn-save" class="btn-default save-btn">
                        <i class="far fa-save"></i>
                        Lưu
                    </button>
                    <!-- <button id="btn-update" class="btn-default update-btn" style="display: none">
                        <i class="far fa-save"></i>
                        Sửa
                    </button> -->
                </div>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'Dialog',
    components: {
    },
    data() {
        return {
            isOpen: true
        }
    },
    methods: {
        closeDialog() {
            this.isOpen = false;
        }
    },
}

</script>