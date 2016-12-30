
# angular

- 限制长度
```javascript
$scope.orderSelect.leaveMessag
var limitation = 50; // 假设文本长度为 50
$scope.$watch('orderSelect.leaveMessage', function(newVal, oldVal) {
	if (newVal && newVal != oldVal) {
		if (newVal.length >= limitation) {
				 $scope.orderSelect.leaveMessage = newVal.substr(0, limitation); // 这里截取有效的50个字符
		}
	}
});
```