# <a name="organization-resource-type"></a><span data-ttu-id="ab8c5-101">organization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ab8c5-101">organization resource type</span></span>

> <span data-ttu-id="ab8c5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ab8c5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab8c5-103">organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。</span><span class="sxs-lookup"><span data-stu-id="ab8c5-103">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="ab8c5-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab8c5-104">Methods</span></span>
|<span data-ttu-id="ab8c5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab8c5-105">Method</span></span>|<span data-ttu-id="ab8c5-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ab8c5-106">Return Type</span></span>|<span data-ttu-id="ab8c5-107">説明</span><span class="sxs-lookup"><span data-stu-id="ab8c5-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ab8c5-108">organizations をリスト</span><span class="sxs-lookup"><span data-stu-id="ab8c5-108">List organizations</span></span>](../api/intune_onboarding_organization_list.md)|<span data-ttu-id="ab8c5-109">[organization](../resources/intune_onboarding_organization.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ab8c5-109">[organization](../resources/intune_onboarding_organization.md) collection</span></span>|<span data-ttu-id="ab8c5-110">[organization](../resources/intune_onboarding_organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ab8c5-110">List properties and relationships of the [organization](../resources/intune_onboarding_organization.md) objects.</span></span>|
|[<span data-ttu-id="ab8c5-111">organization を取得</span><span class="sxs-lookup"><span data-stu-id="ab8c5-111">Get organization</span></span>](../api/intune_onboarding_organization_get.md)|[<span data-ttu-id="ab8c5-112">organization</span><span class="sxs-lookup"><span data-stu-id="ab8c5-112">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="ab8c5-113">[organization](../resources/intune_onboarding_organization.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ab8c5-113">Read properties and relationships of the [organization](../resources/intune_onboarding_organization.md) object.</span></span>|
|[<span data-ttu-id="ab8c5-114">organization の更新</span><span class="sxs-lookup"><span data-stu-id="ab8c5-114">Update organization</span></span>](../api/intune_onboarding_organization_update.md)|[<span data-ttu-id="ab8c5-115">organization</span><span class="sxs-lookup"><span data-stu-id="ab8c5-115">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="ab8c5-116">[organization](../resources/intune_onboarding_organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ab8c5-116">Update the properties of a [organization](../resources/intune_onboarding_organization.md) object.</span></span>|
|[<span data-ttu-id="ab8c5-117">setMobileDeviceManagementAuthority アクション</span><span class="sxs-lookup"><span data-stu-id="ab8c5-117">setMobileDeviceManagementAuthority action</span></span>](../api/intune_onboarding_organization_setmobiledevicemanagementauthority.md)|<span data-ttu-id="ab8c5-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ab8c5-118">Int32</span></span>|<span data-ttu-id="ab8c5-119">モバイル デバイス管理権限の設定</span><span class="sxs-lookup"><span data-stu-id="ab8c5-119">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="ab8c5-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab8c5-120">Properties</span></span>
|<span data-ttu-id="ab8c5-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab8c5-121">Property</span></span>|<span data-ttu-id="ab8c5-122">タイプ</span><span class="sxs-lookup"><span data-stu-id="ab8c5-122">Type</span></span>|<span data-ttu-id="ab8c5-123">説明</span><span class="sxs-lookup"><span data-stu-id="ab8c5-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab8c5-124">id</span><span class="sxs-lookup"><span data-stu-id="ab8c5-124">id</span></span>|<span data-ttu-id="ab8c5-125">文字列</span><span class="sxs-lookup"><span data-stu-id="ab8c5-125">String</span></span>|<span data-ttu-id="ab8c5-126">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="ab8c5-126">The GUID for the object.</span></span>|
|<span data-ttu-id="ab8c5-127">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="ab8c5-127">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="ab8c5-128">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="ab8c5-128">mdmAuthority</span></span>](../resources/intune_onboarding_mdmauthority.md)|<span data-ttu-id="ab8c5-129">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="ab8c5-129">Mobile device management authority.</span></span> <span data-ttu-id="ab8c5-130">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="ab8c5-130">The possible values are `unknown`, `intune`, `sccm`, `office365`, , , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab8c5-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ab8c5-131">Relationships</span></span>
<span data-ttu-id="ab8c5-132">なし</span><span class="sxs-lookup"><span data-stu-id="ab8c5-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ab8c5-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ab8c5-133">JSON Representation</span></span>
<span data-ttu-id="ab8c5-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ab8c5-134">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "openType": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.organization"
}-->
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
    "Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md"
  ]
}-->
