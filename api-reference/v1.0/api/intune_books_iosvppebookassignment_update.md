# <a name="update-iosvppebookassignment"></a><span data-ttu-id="6763b-101">iosVppEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="6763b-101">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="6763b-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6763b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6763b-103">[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6763b-103">Update the properties of a [calendar](../resources/intune_books_iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6763b-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="6763b-104">Prerequisites</span></span>
<span data-ttu-id="6763b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6763b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6763b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6763b-107">Permission type</span></span>|<span data-ttu-id="6763b-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6763b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6763b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6763b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6763b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6763b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6763b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6763b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6763b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6763b-112">Not supported.</span></span>|
|<span data-ttu-id="6763b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6763b-113">Application</span></span>|<span data-ttu-id="6763b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6763b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6763b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6763b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6763b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6763b-116">Request headers</span></span>
|<span data-ttu-id="6763b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6763b-117">Header</span></span>|<span data-ttu-id="6763b-118">値</span><span class="sxs-lookup"><span data-stu-id="6763b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6763b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6763b-119">Authorization</span></span>|<span data-ttu-id="6763b-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6763b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6763b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6763b-121">Accept</span></span>|<span data-ttu-id="6763b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6763b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6763b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6763b-123">Request body</span></span>
<span data-ttu-id="6763b-124">要求本文で、[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6763b-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_books_iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="6763b-125">次の表に、[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6763b-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="6763b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6763b-126">Property</span></span>|<span data-ttu-id="6763b-127">型</span><span class="sxs-lookup"><span data-stu-id="6763b-127">Type</span></span>|<span data-ttu-id="6763b-128">説明</span><span class="sxs-lookup"><span data-stu-id="6763b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6763b-129">id</span><span class="sxs-lookup"><span data-stu-id="6763b-129">id</span></span>|<span data-ttu-id="6763b-130">String</span><span class="sxs-lookup"><span data-stu-id="6763b-130">String</span></span>|<span data-ttu-id="6763b-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6763b-131">Name of the entity.</span></span> <span data-ttu-id="6763b-132">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6763b-132">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="6763b-133">target</span><span class="sxs-lookup"><span data-stu-id="6763b-133">target</span></span>|[<span data-ttu-id="6763b-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6763b-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_books_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6763b-135">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="6763b-135">The assignment target for eBook.</span></span> <span data-ttu-id="6763b-136">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6763b-136">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="6763b-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="6763b-137">installIntent</span></span>|<span data-ttu-id="6763b-138">String</span><span class="sxs-lookup"><span data-stu-id="6763b-138">String</span></span>|<span data-ttu-id="6763b-139">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="6763b-139">The install intent for eBook.</span></span> <span data-ttu-id="6763b-140">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) から継承します。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="6763b-140">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="6763b-141">応答</span><span class="sxs-lookup"><span data-stu-id="6763b-141">Response</span></span>
<span data-ttu-id="6763b-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6763b-142">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_books_iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6763b-143">例</span><span class="sxs-lookup"><span data-stu-id="6763b-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="6763b-144">要求</span><span class="sxs-lookup"><span data-stu-id="6763b-144">Request</span></span>
<span data-ttu-id="6763b-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6763b-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 133

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="6763b-146">応答</span><span class="sxs-lookup"><span data-stu-id="6763b-146">Response</span></span>
<span data-ttu-id="6763b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6763b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



