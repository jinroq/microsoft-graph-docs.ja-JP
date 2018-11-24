# <a name="create-mobileappassignment"></a><span data-ttu-id="7421b-101">mobileAppAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="7421b-101">Create mobileAppAssignment</span></span>

> <span data-ttu-id="7421b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7421b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7421b-103">新しい [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7421b-103">Create a new [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7421b-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="7421b-104">Prerequisites</span></span>
<span data-ttu-id="7421b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7421b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7421b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7421b-107">Permission type</span></span>|<span data-ttu-id="7421b-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7421b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7421b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7421b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7421b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7421b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7421b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7421b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7421b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7421b-112">Not supported.</span></span>|
|<span data-ttu-id="7421b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7421b-113">Application</span></span>|<span data-ttu-id="7421b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7421b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7421b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7421b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7421b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7421b-116">Request headers</span></span>
|<span data-ttu-id="7421b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7421b-117">Header</span></span>|<span data-ttu-id="7421b-118">値</span><span class="sxs-lookup"><span data-stu-id="7421b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7421b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7421b-119">Authorization</span></span>|<span data-ttu-id="7421b-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7421b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7421b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7421b-121">Accept</span></span>|<span data-ttu-id="7421b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7421b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7421b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7421b-123">Request body</span></span>
<span data-ttu-id="7421b-124">要求本文で、mobileAppAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7421b-124">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="7421b-125">次の表に、mobileAppAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7421b-125">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="7421b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7421b-126">Property</span></span>|<span data-ttu-id="7421b-127">型</span><span class="sxs-lookup"><span data-stu-id="7421b-127">Type</span></span>|<span data-ttu-id="7421b-128">説明</span><span class="sxs-lookup"><span data-stu-id="7421b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7421b-129">id</span><span class="sxs-lookup"><span data-stu-id="7421b-129">id</span></span>|<span data-ttu-id="7421b-130">String</span><span class="sxs-lookup"><span data-stu-id="7421b-130">String</span></span>|<span data-ttu-id="7421b-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7421b-131">Key of the entity.</span></span>|
|<span data-ttu-id="7421b-132">intent</span><span class="sxs-lookup"><span data-stu-id="7421b-132">intent</span></span>|[<span data-ttu-id="7421b-133">installIntent</span><span class="sxs-lookup"><span data-stu-id="7421b-133">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="7421b-134">管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="7421b-134">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="7421b-135">target</span><span class="sxs-lookup"><span data-stu-id="7421b-135">target</span></span>|[<span data-ttu-id="7421b-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7421b-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7421b-137">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="7421b-137">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="7421b-138">settings</span><span class="sxs-lookup"><span data-stu-id="7421b-138">settings</span></span>|[<span data-ttu-id="7421b-139">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="7421b-139">mobileAppAssignmentSettings</span></span>](../resources/intune_apps_mobileappassignmentsettings.md)|<span data-ttu-id="7421b-140">管理者によって定義された、ターゲットの割り当ての設定。</span><span class="sxs-lookup"><span data-stu-id="7421b-140">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="7421b-141">応答</span><span class="sxs-lookup"><span data-stu-id="7421b-141">Response</span></span>
<span data-ttu-id="7421b-142">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7421b-142">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7421b-143">例</span><span class="sxs-lookup"><span data-stu-id="7421b-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="7421b-144">要求</span><span class="sxs-lookup"><span data-stu-id="7421b-144">Request</span></span>
<span data-ttu-id="7421b-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7421b-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="7421b-146">応答</span><span class="sxs-lookup"><span data-stu-id="7421b-146">Response</span></span>
<span data-ttu-id="7421b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7421b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



