# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="1a982-101">getManagedAppDiagnosticStatuses 関数</span><span class="sxs-lookup"><span data-stu-id="1a982-101">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="1a982-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a982-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a982-103">特定のユーザーの診断検証状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="1a982-103">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a982-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="1a982-104">Prerequisites</span></span>
<span data-ttu-id="1a982-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a982-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1a982-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a982-107">Permission type</span></span>|<span data-ttu-id="1a982-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a982-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a982-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a982-109">Delegated (work or school account)</span></span>| <span data-ttu-id="1a982-110">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="1a982-110">_varies by context_</span></span>|
| <span data-ttu-id="1a982-111">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="1a982-111">.mam</span></span> | <span data-ttu-id="1a982-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a982-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="1a982-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a982-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a982-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a982-114">Not supported.</span></span>|
|<span data-ttu-id="1a982-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a982-115">Application</span></span>|<span data-ttu-id="1a982-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a982-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a982-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a982-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="1a982-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a982-118">Request headers</span></span>
|<span data-ttu-id="1a982-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a982-119">Header</span></span>|<span data-ttu-id="1a982-120">値</span><span class="sxs-lookup"><span data-stu-id="1a982-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a982-121">承認</span><span class="sxs-lookup"><span data-stu-id="1a982-121">Authorization</span></span>|<span data-ttu-id="1a982-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1a982-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a982-123">承諾する</span><span class="sxs-lookup"><span data-stu-id="1a982-123">Accept</span></span>|<span data-ttu-id="1a982-124">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="1a982-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a982-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a982-125">Request body</span></span>
<span data-ttu-id="1a982-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1a982-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a982-127">応答</span><span class="sxs-lookup"><span data-stu-id="1a982-127">Response</span></span>
<span data-ttu-id="1a982-128">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1a982-128">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a982-129">例</span><span class="sxs-lookup"><span data-stu-id="1a982-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a982-130">要求</span><span class="sxs-lookup"><span data-stu-id="1a982-130">Request</span></span>
<span data-ttu-id="1a982-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a982-131">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="1a982-132">応答</span><span class="sxs-lookup"><span data-stu-id="1a982-132">Response</span></span>
<span data-ttu-id="1a982-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a982-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```



