# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="8a19e-101">groupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a19e-101">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="8a19e-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a19e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a19e-103">グループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="8a19e-103">Represents an assignment to a group.</span></span>

<span data-ttu-id="8a19e-104">[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8a19e-104">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8a19e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a19e-105">Properties</span></span>
|<span data-ttu-id="8a19e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a19e-106">Property</span></span>|<span data-ttu-id="8a19e-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="8a19e-107">Type</span></span>|<span data-ttu-id="8a19e-108">説明</span><span class="sxs-lookup"><span data-stu-id="8a19e-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a19e-109">groupId</span><span class="sxs-lookup"><span data-stu-id="8a19e-109">groupId</span></span>|<span data-ttu-id="8a19e-110">文字列</span><span class="sxs-lookup"><span data-stu-id="8a19e-110">String</span></span>|<span data-ttu-id="8a19e-111">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="8a19e-111">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a19e-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a19e-112">Relationships</span></span>
<span data-ttu-id="8a19e-113">なし</span><span class="sxs-lookup"><span data-stu-id="8a19e-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8a19e-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a19e-114">JSON Representation</span></span>
<span data-ttu-id="8a19e-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8a19e-115">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```








