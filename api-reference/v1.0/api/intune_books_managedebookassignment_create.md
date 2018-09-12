# <a name="create-managedebookassignment"></a><span data-ttu-id="ac6cd-101">managedEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="ac6cd-101">Create managedEBookAssignment</span></span>

> <span data-ttu-id="ac6cd-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac6cd-103">新しい [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-103">Create a new [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac6cd-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ac6cd-104">Prerequisites</span></span>
<span data-ttu-id="ac6cd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ac6cd-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ac6cd-107">Permission type</span></span>|<span data-ttu-id="ac6cd-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ac6cd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac6cd-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ac6cd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ac6cd-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac6cd-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ac6cd-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac6cd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac6cd-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-112">Not supported.</span></span>|
|<span data-ttu-id="ac6cd-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ac6cd-113">Application</span></span>|<span data-ttu-id="ac6cd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac6cd-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ac6cd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ac6cd-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac6cd-116">Request headers</span></span>
|<span data-ttu-id="ac6cd-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac6cd-117">Header</span></span>|<span data-ttu-id="ac6cd-118">値</span><span class="sxs-lookup"><span data-stu-id="ac6cd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac6cd-119">承認</span><span class="sxs-lookup"><span data-stu-id="ac6cd-119">Authorization</span></span>|<span data-ttu-id="ac6cd-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac6cd-121">承諾</span><span class="sxs-lookup"><span data-stu-id="ac6cd-121">Accept</span></span>|<span data-ttu-id="ac6cd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ac6cd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac6cd-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ac6cd-123">Request body</span></span>
<span data-ttu-id="ac6cd-124">要求本文で、managedEBookAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-124">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="ac6cd-125">次の表に、managedEBookAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-125">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="ac6cd-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac6cd-126">Property</span></span>|<span data-ttu-id="ac6cd-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="ac6cd-127">Type</span></span>|<span data-ttu-id="ac6cd-128">説明</span><span class="sxs-lookup"><span data-stu-id="ac6cd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac6cd-129">ID</span><span class="sxs-lookup"><span data-stu-id="ac6cd-129">id</span></span>|<span data-ttu-id="ac6cd-130">文字列</span><span class="sxs-lookup"><span data-stu-id="ac6cd-130">String</span></span>|<span data-ttu-id="ac6cd-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-131">Key of the entity.</span></span>|
|<span data-ttu-id="ac6cd-132">target</span><span class="sxs-lookup"><span data-stu-id="ac6cd-132">target</span></span>|[<span data-ttu-id="ac6cd-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ac6cd-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ac6cd-134">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-134">The assignment target for eBook.</span></span>|
|<span data-ttu-id="ac6cd-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="ac6cd-135">installIntent</span></span>|[<span data-ttu-id="ac6cd-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="ac6cd-136">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="ac6cd-p102">EBook のインストールの目的です。使用可能な値は `available`、 `required`、 `uninstall`、 `availableWithoutEnrollment`です。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-p102">The install intent for eBook. The possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="ac6cd-139">応答</span><span class="sxs-lookup"><span data-stu-id="ac6cd-139">Response</span></span>
<span data-ttu-id="ac6cd-140">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-140">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac6cd-141">例</span><span class="sxs-lookup"><span data-stu-id="ac6cd-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac6cd-142">要求</span><span class="sxs-lookup"><span data-stu-id="ac6cd-142">Request</span></span>
<span data-ttu-id="ac6cd-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ac6cd-144">応答</span><span class="sxs-lookup"><span data-stu-id="ac6cd-144">Response</span></span>
<span data-ttu-id="ac6cd-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ac6cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








