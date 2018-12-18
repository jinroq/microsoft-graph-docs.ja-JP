---
title: getAuditActivityTypes 関数
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: c493c688e4782b848b695fb8383dadb882b28ee2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345984"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="ed129-103">getAuditActivityTypes 関数</span><span class="sxs-lookup"><span data-stu-id="ed129-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="ed129-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ed129-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed129-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ed129-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed129-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ed129-106">Prerequisites</span></span>
<span data-ttu-id="ed129-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed129-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed129-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed129-109">Permission type</span></span>|<span data-ttu-id="ed129-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed129-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed129-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed129-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed129-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed129-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ed129-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed129-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed129-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed129-114">Not supported.</span></span>|
|<span data-ttu-id="ed129-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed129-115">Application</span></span>|<span data-ttu-id="ed129-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed129-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed129-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed129-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="ed129-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed129-118">Request headers</span></span>
|<span data-ttu-id="ed129-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed129-119">Header</span></span>|<span data-ttu-id="ed129-120">値</span><span class="sxs-lookup"><span data-stu-id="ed129-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed129-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed129-121">Authorization</span></span>|<span data-ttu-id="ed129-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ed129-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed129-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ed129-123">Accept</span></span>|<span data-ttu-id="ed129-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ed129-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed129-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed129-125">Request body</span></span>
<span data-ttu-id="ed129-126">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed129-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ed129-127">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="ed129-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ed129-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed129-128">Property</span></span>|<span data-ttu-id="ed129-129">種類</span><span class="sxs-lookup"><span data-stu-id="ed129-129">Type</span></span>|<span data-ttu-id="ed129-130">説明</span><span class="sxs-lookup"><span data-stu-id="ed129-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed129-131">category</span><span class="sxs-lookup"><span data-stu-id="ed129-131">category</span></span>|<span data-ttu-id="ed129-132">String</span><span class="sxs-lookup"><span data-stu-id="ed129-132">String</span></span>|<span data-ttu-id="ed129-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ed129-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ed129-134">応答</span><span class="sxs-lookup"><span data-stu-id="ed129-134">Response</span></span>
<span data-ttu-id="ed129-135">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ed129-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed129-136">例</span><span class="sxs-lookup"><span data-stu-id="ed129-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed129-137">要求</span><span class="sxs-lookup"><span data-stu-id="ed129-137">Request</span></span>
<span data-ttu-id="ed129-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed129-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ed129-139">応答</span><span class="sxs-lookup"><span data-stu-id="ed129-139">Response</span></span>
<span data-ttu-id="ed129-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ed129-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 61

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```



