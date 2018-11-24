# <a name="create-iosvppebookassignment"></a><span data-ttu-id="31c54-101">iosVppEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="31c54-101">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="31c54-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="31c54-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31c54-103">新しい [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="31c54-103">Create a new [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31c54-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="31c54-104">Prerequisites</span></span>
<span data-ttu-id="31c54-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31c54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="31c54-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31c54-107">Permission type</span></span>|<span data-ttu-id="31c54-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="31c54-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31c54-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="31c54-109">Delegated (work or school account)</span></span>|<span data-ttu-id="31c54-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31c54-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="31c54-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31c54-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31c54-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31c54-112">Not supported.</span></span>|
|<span data-ttu-id="31c54-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31c54-113">Application</span></span>|<span data-ttu-id="31c54-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31c54-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31c54-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31c54-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="31c54-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31c54-116">Request headers</span></span>
|<span data-ttu-id="31c54-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31c54-117">Header</span></span>|<span data-ttu-id="31c54-118">値</span><span class="sxs-lookup"><span data-stu-id="31c54-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31c54-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="31c54-119">Authorization</span></span>|<span data-ttu-id="31c54-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="31c54-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31c54-121">Accept</span><span class="sxs-lookup"><span data-stu-id="31c54-121">Accept</span></span>|<span data-ttu-id="31c54-122">application/json</span><span class="sxs-lookup"><span data-stu-id="31c54-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31c54-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="31c54-123">Request body</span></span>
<span data-ttu-id="31c54-124">要求本文で、iosVppEBookAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="31c54-124">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="31c54-125">次の表に、iosVppEBookAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="31c54-125">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="31c54-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31c54-126">Property</span></span>|<span data-ttu-id="31c54-127">型</span><span class="sxs-lookup"><span data-stu-id="31c54-127">Type</span></span>|<span data-ttu-id="31c54-128">説明</span><span class="sxs-lookup"><span data-stu-id="31c54-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31c54-129">id</span><span class="sxs-lookup"><span data-stu-id="31c54-129">id</span></span>|<span data-ttu-id="31c54-130">String</span><span class="sxs-lookup"><span data-stu-id="31c54-130">String</span></span>|<span data-ttu-id="31c54-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="31c54-131">Key of the entity.</span></span> <span data-ttu-id="31c54-132">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31c54-132">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="31c54-133">target</span><span class="sxs-lookup"><span data-stu-id="31c54-133">target</span></span>|[<span data-ttu-id="31c54-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="31c54-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="31c54-135">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="31c54-135">The assignment target for eBook.</span></span> <span data-ttu-id="31c54-136">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31c54-136">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="31c54-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="31c54-137">installIntent</span></span>|[<span data-ttu-id="31c54-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="31c54-138">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="31c54-139">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="31c54-139">The install intent for eBook.</span></span> <span data-ttu-id="31c54-140">[ManagedEBookAssignment](../resources/intune_books_managedebookassignment.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="31c54-140">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span></span> <span data-ttu-id="31c54-141">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="31c54-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="31c54-142">応答</span><span class="sxs-lookup"><span data-stu-id="31c54-142">Response</span></span>
<span data-ttu-id="31c54-143">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="31c54-143">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31c54-144">例</span><span class="sxs-lookup"><span data-stu-id="31c54-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="31c54-145">要求</span><span class="sxs-lookup"><span data-stu-id="31c54-145">Request</span></span>
<span data-ttu-id="31c54-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="31c54-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="31c54-147">応答</span><span class="sxs-lookup"><span data-stu-id="31c54-147">Response</span></span>
<span data-ttu-id="31c54-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="31c54-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "48f05789-5789-48f0-8957-f0488957f048",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



