# <a name="auditproperty-resource-type"></a><span data-ttu-id="d30be-101">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d30be-101">auditProperty resource type</span></span>

> <span data-ttu-id="d30be-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d30be-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d30be-103">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="d30be-103">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="d30be-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d30be-104">Properties</span></span>
|<span data-ttu-id="d30be-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d30be-105">Property</span></span>|<span data-ttu-id="d30be-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="d30be-106">Type</span></span>|<span data-ttu-id="d30be-107">説明</span><span class="sxs-lookup"><span data-stu-id="d30be-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d30be-108">displayName</span><span class="sxs-lookup"><span data-stu-id="d30be-108">displayName</span></span>|<span data-ttu-id="d30be-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d30be-109">String</span></span>|<span data-ttu-id="d30be-110">表示名。</span><span class="sxs-lookup"><span data-stu-id="d30be-110">Display name.</span></span>|
|<span data-ttu-id="d30be-111">oldValue</span><span class="sxs-lookup"><span data-stu-id="d30be-111">oldValue</span></span>|<span data-ttu-id="d30be-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d30be-112">String</span></span>|<span data-ttu-id="d30be-113">以前の値。</span><span class="sxs-lookup"><span data-stu-id="d30be-113">Old value.</span></span>|
|<span data-ttu-id="d30be-114">newValue</span><span class="sxs-lookup"><span data-stu-id="d30be-114">newValue</span></span>|<span data-ttu-id="d30be-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d30be-115">String</span></span>|<span data-ttu-id="d30be-116">新しい値。</span><span class="sxs-lookup"><span data-stu-id="d30be-116">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d30be-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d30be-117">Relationships</span></span>
<span data-ttu-id="d30be-118">なし</span><span class="sxs-lookup"><span data-stu-id="d30be-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d30be-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d30be-119">JSON Representation</span></span>
<span data-ttu-id="d30be-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d30be-120">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



