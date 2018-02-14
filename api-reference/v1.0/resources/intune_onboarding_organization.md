# <a name="organization-resource-type"></a><span data-ttu-id="55502-101">organization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="55502-101">organization resource type</span></span>

> <span data-ttu-id="55502-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="55502-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55502-103">organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。</span><span class="sxs-lookup"><span data-stu-id="55502-103">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="55502-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="55502-104">Methods</span></span>
|<span data-ttu-id="55502-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="55502-105">Method</span></span>|<span data-ttu-id="55502-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="55502-106">Return Type</span></span>|<span data-ttu-id="55502-107">説明</span><span class="sxs-lookup"><span data-stu-id="55502-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="55502-108">List organizations</span><span class="sxs-lookup"><span data-stu-id="55502-108">List organizations</span></span>](../api/intune_onboarding_organization_list.md)|<span data-ttu-id="55502-109">[organization](../resources/intune_onboarding_organization.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="55502-109">[organization](../resources/intune_onboarding_organization.md) collection</span></span>|<span data-ttu-id="55502-110">[organization](../resources/intune_onboarding_organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="55502-110">List properties and relationships of the [organization](../resources/intune_onboarding_organization.md) objects.</span></span>|
|[<span data-ttu-id="55502-111">Get organization</span><span class="sxs-lookup"><span data-stu-id="55502-111">Get organization</span></span>](../api/intune_onboarding_organization_get.md)|[<span data-ttu-id="55502-112">organization</span><span class="sxs-lookup"><span data-stu-id="55502-112">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="55502-113">[organization](../resources/intune_onboarding_organization.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="55502-113">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="55502-114">Update organization</span><span class="sxs-lookup"><span data-stu-id="55502-114">Update organization</span></span>](../api/intune_onboarding_organization_update.md)|[<span data-ttu-id="55502-115">organization</span><span class="sxs-lookup"><span data-stu-id="55502-115">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="55502-116">[organization](../resources/intune_onboarding_organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="55502-116">Update the properties of a [calendar](../resources/intune_onboarding_organization.md) object.</span></span>|
|[<span data-ttu-id="55502-117">setMobileDeviceManagementAuthority アクション</span><span class="sxs-lookup"><span data-stu-id="55502-117">setMobileDeviceManagementAuthority action</span></span>](../api/intune_onboarding_organization_setmobiledevicemanagementauthority.md)|<span data-ttu-id="55502-118">Int32</span><span class="sxs-lookup"><span data-stu-id="55502-118">Int32</span></span>|<span data-ttu-id="55502-119">モバイル デバイス管理権限の設定</span><span class="sxs-lookup"><span data-stu-id="55502-119">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="55502-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55502-120">Properties</span></span>
|<span data-ttu-id="55502-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55502-121">Property</span></span>|<span data-ttu-id="55502-122">型</span><span class="sxs-lookup"><span data-stu-id="55502-122">Type</span></span>|<span data-ttu-id="55502-123">説明</span><span class="sxs-lookup"><span data-stu-id="55502-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55502-124">id</span><span class="sxs-lookup"><span data-stu-id="55502-124">id</span></span>|<span data-ttu-id="55502-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="55502-125">String</span></span>|<span data-ttu-id="55502-126">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="55502-126">The user GUID for the security object is not valid.</span></span>|
|<span data-ttu-id="55502-127">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="55502-127">mobileDeviceManagementAuthority</span></span>|<span data-ttu-id="55502-128">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="55502-128">String</span></span>|<span data-ttu-id="55502-129">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="55502-129">Mobile device management authority.</span></span> <span data-ttu-id="55502-130">可能な値: `unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="55502-130">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55502-131">関係</span><span class="sxs-lookup"><span data-stu-id="55502-131">Relationships</span></span>
<span data-ttu-id="55502-132">なし</span><span class="sxs-lookup"><span data-stu-id="55502-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="55502-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="55502-133">JSON Representation</span></span>
<span data-ttu-id="55502-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="55502-134">Here is a JSON representation of the resource.</span></span>
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



