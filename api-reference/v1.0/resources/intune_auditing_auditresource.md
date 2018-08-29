# <a name="auditresource-resource-type"></a><span data-ttu-id="fa57e-101">auditResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa57e-101">auditResource resource type</span></span>

> <span data-ttu-id="fa57e-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fa57e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa57e-103">監査のリソースのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="fa57e-103">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="fa57e-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa57e-104">Properties</span></span>
|<span data-ttu-id="fa57e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa57e-105">Property</span></span>|<span data-ttu-id="fa57e-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="fa57e-106">Type</span></span>|<span data-ttu-id="fa57e-107">説明</span><span class="sxs-lookup"><span data-stu-id="fa57e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa57e-108">displayName</span><span class="sxs-lookup"><span data-stu-id="fa57e-108">displayName</span></span>|<span data-ttu-id="fa57e-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fa57e-109">String</span></span>|<span data-ttu-id="fa57e-110">表示名。</span><span class="sxs-lookup"><span data-stu-id="fa57e-110">Display name.</span></span>|
|<span data-ttu-id="fa57e-111">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="fa57e-111">modifiedProperties</span></span>|<span data-ttu-id="fa57e-112">[auditProperty](../resources/intune_auditing_auditproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fa57e-112">[auditProperty](../resources/intune_auditing_auditproperty.md) collection</span></span>|<span data-ttu-id="fa57e-113">変更されたプロパティの一覧。</span><span class="sxs-lookup"><span data-stu-id="fa57e-113">List of modified properties.</span></span>|
|<span data-ttu-id="fa57e-114">type</span><span class="sxs-lookup"><span data-stu-id="fa57e-114">type</span></span>|<span data-ttu-id="fa57e-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fa57e-115">String</span></span>|<span data-ttu-id="fa57e-116">監査のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="fa57e-116">Audit resource's type.</span></span>|
|<span data-ttu-id="fa57e-117">resourceId</span><span class="sxs-lookup"><span data-stu-id="fa57e-117">resourceId</span></span>|<span data-ttu-id="fa57e-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fa57e-118">String</span></span>|<span data-ttu-id="fa57e-119">監査のリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="fa57e-119">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa57e-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fa57e-120">Relationships</span></span>
<span data-ttu-id="fa57e-121">なし</span><span class="sxs-lookup"><span data-stu-id="fa57e-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fa57e-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa57e-122">JSON Representation</span></span>
<span data-ttu-id="fa57e-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fa57e-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}-->
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



