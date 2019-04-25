---
title: managedDeviceEnrollmentFailureTrends 関数
description: 登録失敗傾向レポートのメタデータ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e5d15c247c16e22748da0fe0db358adbe41035f9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526973"
---
# <a name="manageddeviceenrollmentfailuretrends-function"></a><span data-ttu-id="a432b-103">managedDeviceEnrollmentFailureTrends 関数</span><span class="sxs-lookup"><span data-stu-id="a432b-103">managedDeviceEnrollmentFailureTrends function</span></span>

> <span data-ttu-id="a432b-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a432b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a432b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a432b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a432b-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a432b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a432b-107">登録失敗傾向レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="a432b-107">Metadata for the enrollment failure trends report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a432b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a432b-108">Prerequisites</span></span>
<span data-ttu-id="a432b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a432b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a432b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a432b-111">Permission type</span></span>|<span data-ttu-id="a432b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a432b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a432b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a432b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a432b-114">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="a432b-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a432b-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a432b-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a432b-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a432b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a432b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a432b-117">Not supported.</span></span>|
|<span data-ttu-id="a432b-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a432b-118">Application</span></span>|<span data-ttu-id="a432b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a432b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a432b-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a432b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureTrends
```

## <a name="request-headers"></a><span data-ttu-id="a432b-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a432b-121">Request headers</span></span>
|<span data-ttu-id="a432b-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a432b-122">Header</span></span>|<span data-ttu-id="a432b-123">値</span><span class="sxs-lookup"><span data-stu-id="a432b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a432b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a432b-124">Authorization</span></span>|<span data-ttu-id="a432b-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a432b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a432b-126">承諾</span><span class="sxs-lookup"><span data-stu-id="a432b-126">Accept</span></span>|<span data-ttu-id="a432b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a432b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a432b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a432b-128">Request body</span></span>
<span data-ttu-id="a432b-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a432b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a432b-130">応答</span><span class="sxs-lookup"><span data-stu-id="a432b-130">Response</span></span>
<span data-ttu-id="a432b-131">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="a432b-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a432b-132">例</span><span class="sxs-lookup"><span data-stu-id="a432b-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="a432b-133">要求</span><span class="sxs-lookup"><span data-stu-id="a432b-133">Request</span></span>
<span data-ttu-id="a432b-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a432b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureTrends
```

### <a name="response"></a><span data-ttu-id="a432b-135">応答</span><span class="sxs-lookup"><span data-stu-id="a432b-135">Response</span></span>
<span data-ttu-id="a432b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a432b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```



