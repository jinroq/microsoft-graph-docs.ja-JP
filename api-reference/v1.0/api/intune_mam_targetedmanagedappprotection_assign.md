# <a name="assign-action"></a><span data-ttu-id="33392-101">assign アクション</span><span class="sxs-lookup"><span data-stu-id="33392-101">assign action</span></span>

> <span data-ttu-id="33392-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="33392-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33392-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="33392-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33392-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="33392-104">Prerequisites</span></span>
<span data-ttu-id="33392-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33392-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="33392-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33392-107">Permission type</span></span>|<span data-ttu-id="33392-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="33392-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33392-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33392-109">Delegated (work or school account)</span></span>|<span data-ttu-id="33392-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33392-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="33392-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33392-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33392-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33392-112">Not supported.</span></span>|
|<span data-ttu-id="33392-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33392-113">Application</span></span>|<span data-ttu-id="33392-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33392-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33392-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33392-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="33392-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33392-116">Request headers</span></span>
|<span data-ttu-id="33392-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33392-117">Header</span></span>|<span data-ttu-id="33392-118">値</span><span class="sxs-lookup"><span data-stu-id="33392-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33392-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="33392-119">Authorization</span></span>|<span data-ttu-id="33392-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="33392-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33392-121">Accept</span><span class="sxs-lookup"><span data-stu-id="33392-121">Accept</span></span>|<span data-ttu-id="33392-122">application/json</span><span class="sxs-lookup"><span data-stu-id="33392-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33392-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="33392-123">Request body</span></span>
<span data-ttu-id="33392-124">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="33392-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="33392-125">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="33392-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="33392-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33392-126">Property</span></span>|<span data-ttu-id="33392-127">Type</span><span class="sxs-lookup"><span data-stu-id="33392-127">Type</span></span>|<span data-ttu-id="33392-128">説明</span><span class="sxs-lookup"><span data-stu-id="33392-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33392-129">assignments</span><span class="sxs-lookup"><span data-stu-id="33392-129">assignments</span></span>|<span data-ttu-id="33392-130">[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="33392-130">[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="33392-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="33392-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="33392-132">応答</span><span class="sxs-lookup"><span data-stu-id="33392-132">Response</span></span>
<span data-ttu-id="33392-133">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="33392-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="33392-134">例</span><span class="sxs-lookup"><span data-stu-id="33392-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="33392-135">要求</span><span class="sxs-lookup"><span data-stu-id="33392-135">Request</span></span>
<span data-ttu-id="33392-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="33392-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

Content-type: application/json
Content-length: 282

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="33392-137">応答</span><span class="sxs-lookup"><span data-stu-id="33392-137">Response</span></span>
<span data-ttu-id="33392-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="33392-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



