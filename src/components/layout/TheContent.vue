<template>
    <div id="content">
        <!-- <div class="page-title">
            <div class="page-left">Danh sách khách hàng</div>
            <div class="page-right">
                <button id="btn-add" class="btn-default add-customer-btn">Thêm khách hàng</button>
            </div>
        </div>
        <div class="toolbar">
            <input type="text" class="input-search" placeholder="Tìm kiếm theo mã, tên khách hàng" />
            <button class="btn-refresh"></button>
            <button class="btn-delete">Xóa</button>
        </div>

        <div class="grid">
            <table id="tblClassListCustomer" class="table" width="100%" border="0">
                <thead>
                    <tr>
                        <th>Mã khách hàng</th>
                        <th>Họ và tên</th>
                        <th>Giới tính</th>
                        <th>Ngày sinh</th>
                        <th>Nhóm khách hàng</th>
                        <th>Điện thoại</th>
                        <th>Email</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>MF3213</td>
                        <td>Ngọc Dũng</td>
                        <td>Nam</td>
                        <td>12/11/2000</td>
                        <td>Khách VIP</td>
                        <td>086834090</td>
                        <td>dungbachngoc20@gmail.com</td>
                    </tr>
                    <tr>
                        <td>MF3213</td>
                        <td>Ngọc Dũng</td>
                        <td>Nam</td>
                        <td>12/11/2000</td>
                        <td>Khách VIP</td>
                        <td>086834090</td>
                        <td>dungbachngoc20@gmail.com</td>
                    </tr>
                    <tr>
                        <td>MF3213</td>
                        <td>Ngọc Dũng</td>
                        <td>Nam</td>
                        <td>12/11/2000</td>
                        <td>Khách VIP</td>
                        <td>086834090</td>
                        <td>dungbachngoc20@gmail.com</td>
                    </tr>
                </tbody>
            </table>
        </div> -->
        <CustomerDetail />
        <CustomerList />
        <TheFooter />
    </div>
</template>

<script>
import TheFooter from './TheFooter.vue'
import CustomerDetail from '../../views/customer/CustomerDetail.vue'
import CustomerList from '../../views/customer/CustomerList.vue'

export default {
    name: 'Content',
    components: {
        TheFooter,
        CustomerDetail,
        CustomerList
    }
}

</script>

<style scoped>
#content{
    position: absolute;
    top: 60px;
    left: 200px;
    right: 0px;
    bottom: 0px;
    padding: 24px;
}
</style>