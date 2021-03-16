<template>
    <div> 
         <div class="page-title">
        <div class="page-left">Danh sách Nhân viên</div>
        <div class="page-right">
          <button id="btnAdd" class="btn-default">Thêm khách hàng</button>
        </div>
      </div>
      <div class="toolbar">
        <input
          type="text"
          class="input-search"
          placeholder="Tìm kiếm theo mã, tên khách hàng"
        />
        <button class="btn-refresh"></button>
      </div>
      <div class="grid">
        <table class="table" width="100%" border="0">
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
              <td>KH0001</td>
              <td>Nguyễn Văn Mạnh</td>
              <td>Nam</td>
              <td>22/09/1999</td>
              <td>VIP</td>
              <td>0961179969</td>
              <td>manhnv229@gmail.com</td>
            </tr>
            <tr>
              <td>KH0001</td>
              <td>Nguyễn Văn Mạnh</td>
              <td>Nam</td>
              <td>22/09/1999</td>
              <td>VIP</td>
              <td>0961179969</td>
              <td>manhnv229@gmail.com</td>
            </tr>
            <tr>
              <td>KH0001</td>
              <td>Nguyễn Văn Mạnh</td>
              <td>Nam</td>
              <td>22/09/1999</td>
              <td>VIP</td>
              <td>0961179969</td>
              <td>manhnv229@gmail.com</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="paging"></div>
      <EmployeeListDetail/>
    </div>
    
</template>
<script>
import EmployeeListDetail from "./EmployeeListDetail.vue";
export default {
  name: "Employee",
  components: {
    EmployeeListDetail
  },
};
</script>
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

.grid{
    position: absolute;
    /* height: 4000px; */
    /* background-color: aqua; */
    /* width: 100%; */
    right:  24px;
    left: 24px;
    bottom: 60px;
    top: 128px;
}

.paging{
    position: absolute;
    bottom:0;
    height: 60px;
    background-color: aquamarine;
    left: 24px;
    right: 24px;
}
</style>