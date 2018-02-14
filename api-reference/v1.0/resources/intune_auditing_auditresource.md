# <a name="auditresource-resource-type"></a><span data-ttu-id="36074-101">auditResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="36074-101">auditResource resource type</span></span>

> <span data-ttu-id="36074-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="36074-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36074-103">監査のリソースのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="36074-103">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="36074-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36074-104">Properties</span></span>
|<span data-ttu-id="36074-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36074-105">Property</span></span>|<span data-ttu-id="36074-106">型</span><span class="sxs-lookup"><span data-stu-id="36074-106">Type</span></span>|<span data-ttu-id="36074-107">説明</span><span class="sxs-lookup"><span data-stu-id="36074-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36074-108">displayName</span><span class="sxs-lookup"><span data-stu-id="36074-108">displayName</span></span>|<span data-ttu-id="36074-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="36074-109">String</span></span>|<span data-ttu-id="36074-110">表示名。</span><span class="sxs-lookup"><span data-stu-id="36074-110">Display Name</span></span>|
|<span data-ttu-id="36074-111">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="36074-111">ModifiedProperties</span></span>|<span data-ttu-id="36074-112">[auditProperty](../resources/intune_auditing_auditproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="36074-112">[auditProperty](../resources/intune_auditing_auditproperty.md) collection</span></span>|<span data-ttu-id="36074-113">変更されたプロパティの一覧。</span><span class="sxs-lookup"><span data-stu-id="36074-113">List of managed properties</span></span>|
|<span data-ttu-id="36074-114">type</span><span class="sxs-lookup"><span data-stu-id="36074-114">type</span></span>|<span data-ttu-id="36074-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="36074-115">String</span></span>|<span data-ttu-id="36074-116">監査のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="36074-116">Audit resource's type.</span></span>|
|<span data-ttu-id="36074-117">resourceId</span><span class="sxs-lookup"><span data-stu-id="36074-117">resourceId</span></span>|<span data-ttu-id="36074-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="36074-118">String</span></span>|<span data-ttu-id="36074-119">監査のリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="36074-119">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36074-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="36074-120">Relationships</span></span>
<span data-ttu-id="36074-121">なし</span><span class="sxs-lookup"><span data-stu-id="36074-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="36074-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="36074-122">JSON Representation</span></span>
<span data-ttu-id="36074-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="36074-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```



