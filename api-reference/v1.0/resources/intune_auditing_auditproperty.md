# <a name="auditproperty-resource-type"></a><span data-ttu-id="399d3-101">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="399d3-101">auditProperty resource type</span></span>

> <span data-ttu-id="399d3-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="399d3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="399d3-103">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="399d3-103">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="399d3-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="399d3-104">Properties</span></span>
|<span data-ttu-id="399d3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="399d3-105">Property</span></span>|<span data-ttu-id="399d3-106">型</span><span class="sxs-lookup"><span data-stu-id="399d3-106">Type</span></span>|<span data-ttu-id="399d3-107">説明</span><span class="sxs-lookup"><span data-stu-id="399d3-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="399d3-108">displayName</span><span class="sxs-lookup"><span data-stu-id="399d3-108">displayName</span></span>|<span data-ttu-id="399d3-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="399d3-109">String</span></span>|<span data-ttu-id="399d3-110">表示名。</span><span class="sxs-lookup"><span data-stu-id="399d3-110">Display name.</span></span>|
|<span data-ttu-id="399d3-111">oldValue</span><span class="sxs-lookup"><span data-stu-id="399d3-111">oldValue</span></span>|<span data-ttu-id="399d3-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="399d3-112">String</span></span>|<span data-ttu-id="399d3-113">以前の値。</span><span class="sxs-lookup"><span data-stu-id="399d3-113">Old value.</span></span>|
|<span data-ttu-id="399d3-114">newValue</span><span class="sxs-lookup"><span data-stu-id="399d3-114">newValue</span></span>|<span data-ttu-id="399d3-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="399d3-115">String</span></span>|<span data-ttu-id="399d3-116">新しい値。</span><span class="sxs-lookup"><span data-stu-id="399d3-116">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="399d3-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="399d3-117">Relationships</span></span>
<span data-ttu-id="399d3-118">なし</span><span class="sxs-lookup"><span data-stu-id="399d3-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="399d3-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="399d3-119">JSON Representation</span></span>
<span data-ttu-id="399d3-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="399d3-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



