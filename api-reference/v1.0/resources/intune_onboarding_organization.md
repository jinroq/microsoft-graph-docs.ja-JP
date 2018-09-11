# <a name="organization-resource-type"></a><span data-ttu-id="e4f18-101">organization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e4f18-101">organization resource type</span></span>

> <span data-ttu-id="e4f18-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4f18-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4f18-103">organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。</span><span class="sxs-lookup"><span data-stu-id="e4f18-103">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="e4f18-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="e4f18-104">Methods</span></span>
|<span data-ttu-id="e4f18-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e4f18-105">Method</span></span>|<span data-ttu-id="e4f18-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e4f18-106">Return Type</span></span>|<span data-ttu-id="e4f18-107">説明</span><span class="sxs-lookup"><span data-stu-id="e4f18-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e4f18-108">organizations をリスト</span><span class="sxs-lookup"><span data-stu-id="e4f18-108">List organizations</span></span>](../api/intune_onboarding_organization_list.md)|<span data-ttu-id="e4f18-109">[organization](../resources/intune_onboarding_organization.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e4f18-109">[organization](../resources/intune_onboarding_organization.md) collection</span></span>|<span data-ttu-id="e4f18-110">[organization](../resources/intune_onboarding_organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e4f18-110">List properties and relationships of the [organization](../resources/intune_onboarding_organization.md) objects.</span></span>|
|[<span data-ttu-id="e4f18-111">organization を取得</span><span class="sxs-lookup"><span data-stu-id="e4f18-111">Get organization</span></span>](../api/intune_onboarding_organization_get.md)|[<span data-ttu-id="e4f18-112">組織
</span><span class="sxs-lookup"><span data-stu-id="e4f18-112">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="e4f18-113">[organization](../resources/intune_onboarding_organization.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e4f18-113">Read properties and relationships of the [organization](../resources/intune_onboarding_organization.md) object.</span></span>|
|[<span data-ttu-id="e4f18-114">organization の更新</span><span class="sxs-lookup"><span data-stu-id="e4f18-114">Update organization</span></span>](../api/intune_onboarding_organization_update.md)|[<span data-ttu-id="e4f18-115">組織
</span><span class="sxs-lookup"><span data-stu-id="e4f18-115">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="e4f18-116">[organization](../resources/intune_onboarding_organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e4f18-116">Update the properties of a [organization](../resources/intune_onboarding_organization.md) object.</span></span>|
|[<span data-ttu-id="e4f18-117">setMobileDeviceManagementAuthority アクション</span><span class="sxs-lookup"><span data-stu-id="e4f18-117">setMobileDeviceManagementAuthority action</span></span>](../api/intune_onboarding_organization_setmobiledevicemanagementauthority.md)|<span data-ttu-id="e4f18-118">Int32</span><span class="sxs-lookup"><span data-stu-id="e4f18-118">Int32</span></span>|<span data-ttu-id="e4f18-119">モバイル デバイス管理権限の設定</span><span class="sxs-lookup"><span data-stu-id="e4f18-119">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="e4f18-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4f18-120">Properties</span></span>
|<span data-ttu-id="e4f18-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4f18-121">Property</span></span>|<span data-ttu-id="e4f18-122">タイプ</span><span class="sxs-lookup"><span data-stu-id="e4f18-122">Type</span></span>|<span data-ttu-id="e4f18-123">説明</span><span class="sxs-lookup"><span data-stu-id="e4f18-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4f18-124">id</span><span class="sxs-lookup"><span data-stu-id="e4f18-124">id</span></span>|<span data-ttu-id="e4f18-125">文字列</span><span class="sxs-lookup"><span data-stu-id="e4f18-125">String</span></span>|<span data-ttu-id="e4f18-126">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="e4f18-126">The GUID for the object.</span></span>|
|<span data-ttu-id="e4f18-127">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e4f18-127">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="e4f18-128">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="e4f18-128">mdmAuthority</span></span>](../resources/intune_onboarding_mdmauthority.md)|<span data-ttu-id="e4f18-p101">モバイル デバイス管理権限。指定できる値は、`unknown` 、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="e4f18-p101">Mobile device management authority. The possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4f18-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e4f18-131">Relationships</span></span>
<span data-ttu-id="e4f18-132">なし</span><span class="sxs-lookup"><span data-stu-id="e4f18-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e4f18-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e4f18-133">JSON Representation</span></span>
<span data-ttu-id="e4f18-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e4f18-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md",

"Warning: Schema type organization has a different BaseType value microsoft.graph.directoryObject than the documentation .",

"Warning: Schema type organization has a different OpenType value False than the documentation True.",

"Warning: Resource organization has multiple declarations with mismatched OpenType declarations."

  ],

}
-->






