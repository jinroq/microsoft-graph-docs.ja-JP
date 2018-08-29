# <a name="rolepermission-resource-type"></a><span data-ttu-id="0e0ba-101">rolePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0e0ba-101">rolePermission resource type</span></span>

> <span data-ttu-id="0e0ba-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0e0ba-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e0ba-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0e0ba-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0e0ba-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e0ba-104">Properties</span></span>
|<span data-ttu-id="0e0ba-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e0ba-105">Property</span></span>|<span data-ttu-id="0e0ba-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="0e0ba-106">Type</span></span>|<span data-ttu-id="0e0ba-107">説明</span><span class="sxs-lookup"><span data-stu-id="0e0ba-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e0ba-108">resourceActions</span><span class="sxs-lookup"><span data-stu-id="0e0ba-108">resourceActions</span></span>|<span data-ttu-id="0e0ba-109">[resourceAction](../resources/intune_rbac_resourceaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0e0ba-109">[resourceAction](../resources/intune_rbac_resourceaction.md) collection</span></span>|<span data-ttu-id="0e0ba-110">アクション</span><span class="sxs-lookup"><span data-stu-id="0e0ba-110">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e0ba-111">関係</span><span class="sxs-lookup"><span data-stu-id="0e0ba-111">Relationships</span></span>
<span data-ttu-id="0e0ba-112">なし</span><span class="sxs-lookup"><span data-stu-id="0e0ba-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0e0ba-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e0ba-113">JSON Representation</span></span>
<span data-ttu-id="0e0ba-114">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0e0ba-114">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```



