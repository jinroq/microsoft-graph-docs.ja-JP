# <a name="rolepermission-resource-type"></a><span data-ttu-id="3a0a8-101">rolePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3a0a8-101">rolePermission resource type</span></span>

> <span data-ttu-id="3a0a8-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3a0a8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a0a8-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3a0a8-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3a0a8-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a0a8-104">Properties</span></span>
|<span data-ttu-id="3a0a8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a0a8-105">Property</span></span>|<span data-ttu-id="3a0a8-106">型</span><span class="sxs-lookup"><span data-stu-id="3a0a8-106">Type</span></span>|<span data-ttu-id="3a0a8-107">説明</span><span class="sxs-lookup"><span data-stu-id="3a0a8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a0a8-108">resourceActions</span><span class="sxs-lookup"><span data-stu-id="3a0a8-108">resourceActions</span></span>|<span data-ttu-id="3a0a8-109">[resourceAction](../resources/intune_rbac_resourceaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3a0a8-109">[resourceAction](../resources/intune_rbac_resourceaction.md) collection</span></span>|<span data-ttu-id="3a0a8-110">アクション</span><span class="sxs-lookup"><span data-stu-id="3a0a8-110">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a0a8-111">関係</span><span class="sxs-lookup"><span data-stu-id="3a0a8-111">Relationships</span></span>
<span data-ttu-id="3a0a8-112">なし</span><span class="sxs-lookup"><span data-stu-id="3a0a8-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3a0a8-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3a0a8-113">JSON Representation</span></span>
<span data-ttu-id="3a0a8-114">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3a0a8-114">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



