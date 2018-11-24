# <a name="assign-action"></a><span data-ttu-id="099df-101">assign アクション</span><span class="sxs-lookup"><span data-stu-id="099df-101">assign action</span></span>

> <span data-ttu-id="099df-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="099df-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="099df-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="099df-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="099df-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="099df-104">Prerequisites</span></span>
<span data-ttu-id="099df-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="099df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="099df-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="099df-107">Permission type</span></span>|<span data-ttu-id="099df-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="099df-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="099df-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="099df-109">Delegated (work or school account)</span></span>|<span data-ttu-id="099df-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="099df-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="099df-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="099df-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="099df-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="099df-112">Not supported.</span></span>|
|<span data-ttu-id="099df-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="099df-113">Application</span></span>|<span data-ttu-id="099df-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="099df-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="099df-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="099df-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="099df-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="099df-116">Request headers</span></span>
|<span data-ttu-id="099df-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="099df-117">Header</span></span>|<span data-ttu-id="099df-118">値</span><span class="sxs-lookup"><span data-stu-id="099df-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="099df-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="099df-119">Authorization</span></span>|<span data-ttu-id="099df-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="099df-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="099df-121">Accept</span><span class="sxs-lookup"><span data-stu-id="099df-121">Accept</span></span>|<span data-ttu-id="099df-122">application/json</span><span class="sxs-lookup"><span data-stu-id="099df-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="099df-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="099df-123">Request body</span></span>
<span data-ttu-id="099df-124">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="099df-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="099df-125">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="099df-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="099df-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="099df-126">Property</span></span>|<span data-ttu-id="099df-127">型</span><span class="sxs-lookup"><span data-stu-id="099df-127">Type</span></span>|<span data-ttu-id="099df-128">説明</span><span class="sxs-lookup"><span data-stu-id="099df-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="099df-129">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="099df-129">managedEBookAssignments</span></span>|<span data-ttu-id="099df-130">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="099df-130">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) collection</span></span>|<span data-ttu-id="099df-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="099df-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="099df-132">応答</span><span class="sxs-lookup"><span data-stu-id="099df-132">Response</span></span>
<span data-ttu-id="099df-133">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="099df-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="099df-134">例</span><span class="sxs-lookup"><span data-stu-id="099df-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="099df-135">要求</span><span class="sxs-lookup"><span data-stu-id="099df-135">Request</span></span>
<span data-ttu-id="099df-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="099df-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assign

Content-type: application/json
Content-length: 318

{
  "managedEBookAssignments": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="099df-137">応答</span><span class="sxs-lookup"><span data-stu-id="099df-137">Response</span></span>
<span data-ttu-id="099df-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="099df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



