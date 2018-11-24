# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="bb08b-101">exclusionGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb08b-101">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="bb08b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bb08b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb08b-103">割り当てから除外するグループを表します。</span><span class="sxs-lookup"><span data-stu-id="bb08b-103">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="bb08b-104">[groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bb08b-104">Inherits from [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bb08b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb08b-105">Properties</span></span>
|<span data-ttu-id="bb08b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb08b-106">Property</span></span>|<span data-ttu-id="bb08b-107">型</span><span class="sxs-lookup"><span data-stu-id="bb08b-107">Type</span></span>|<span data-ttu-id="bb08b-108">説明</span><span class="sxs-lookup"><span data-stu-id="bb08b-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb08b-109">groupId</span><span class="sxs-lookup"><span data-stu-id="bb08b-109">groupId</span></span>|<span data-ttu-id="bb08b-110">文字列</span><span class="sxs-lookup"><span data-stu-id="bb08b-110">String</span></span>|<span data-ttu-id="bb08b-111">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="bb08b-111">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="bb08b-112">[groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bb08b-112">Inherited from [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb08b-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb08b-113">Relationships</span></span>
<span data-ttu-id="bb08b-114">なし</span><span class="sxs-lookup"><span data-stu-id="bb08b-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bb08b-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb08b-115">JSON Representation</span></span>
<span data-ttu-id="bb08b-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb08b-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



