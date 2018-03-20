# <a name="create-managedebookassignment"></a><span data-ttu-id="26091-101">managedEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="26091-101">Create managedEBookAssignment</span></span>

> <span data-ttu-id="26091-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="26091-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26091-103">新しい [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="26091-103">Create a new [plannerBucket](../resources/intune_books_managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="26091-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="26091-104">Prerequisites</span></span>
<span data-ttu-id="26091-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="26091-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26091-107">Permission type</span></span>|<span data-ttu-id="26091-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="26091-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26091-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26091-109">Delegated (work or school account)</span></span>|<span data-ttu-id="26091-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26091-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="26091-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26091-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26091-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26091-112">Not supported.</span></span>|
|<span data-ttu-id="26091-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26091-113">Application</span></span>|<span data-ttu-id="26091-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26091-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26091-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26091-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="26091-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26091-116">Request headers</span></span>
|<span data-ttu-id="26091-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26091-117">Header</span></span>|<span data-ttu-id="26091-118">値</span><span class="sxs-lookup"><span data-stu-id="26091-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26091-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="26091-119">Authorization</span></span>|<span data-ttu-id="26091-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="26091-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="26091-121">Accept</span><span class="sxs-lookup"><span data-stu-id="26091-121">Accept</span></span>|<span data-ttu-id="26091-122">application/json</span><span class="sxs-lookup"><span data-stu-id="26091-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26091-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="26091-123">Request body</span></span>
<span data-ttu-id="26091-124">要求本文で、managedEBookAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="26091-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="26091-125">次の表に、managedEBookAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="26091-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="26091-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26091-126">Property</span></span>|<span data-ttu-id="26091-127">型</span><span class="sxs-lookup"><span data-stu-id="26091-127">Type</span></span>|<span data-ttu-id="26091-128">説明</span><span class="sxs-lookup"><span data-stu-id="26091-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26091-129">id</span><span class="sxs-lookup"><span data-stu-id="26091-129">id</span></span>|<span data-ttu-id="26091-130">String</span><span class="sxs-lookup"><span data-stu-id="26091-130">String</span></span>|<span data-ttu-id="26091-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="26091-131">Name of the entity.</span></span>|
|<span data-ttu-id="26091-132">target</span><span class="sxs-lookup"><span data-stu-id="26091-132">target</span></span>|[<span data-ttu-id="26091-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="26091-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_books_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="26091-134">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="26091-134">The assignment target for eBook.</span></span>|
|<span data-ttu-id="26091-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="26091-135">installIntent</span></span>|<span data-ttu-id="26091-136">String</span><span class="sxs-lookup"><span data-stu-id="26091-136">String</span></span>|<span data-ttu-id="26091-137">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="26091-137">The install intent for eBook.</span></span> <span data-ttu-id="26091-138">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="26091-138">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="26091-139">応答</span><span class="sxs-lookup"><span data-stu-id="26091-139">Response</span></span>
<span data-ttu-id="26091-140">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="26091-140">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_books_managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26091-141">例</span><span class="sxs-lookup"><span data-stu-id="26091-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="26091-142">要求</span><span class="sxs-lookup"><span data-stu-id="26091-142">Request</span></span>
<span data-ttu-id="26091-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="26091-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="26091-144">応答</span><span class="sxs-lookup"><span data-stu-id="26091-144">Response</span></span>
<span data-ttu-id="26091-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="26091-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



