---
title: deviceConfigurationUserActivity 関数
description: デバイス構成のユーザー アクティビティ レポートのメタデータ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5d2fbaf3224bb1a1949bb2161694e40568225d1b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025863"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="24cf9-103">deviceConfigurationUserActivity 関数</span><span class="sxs-lookup"><span data-stu-id="24cf9-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="24cf9-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="24cf9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24cf9-105">デバイス構成のユーザー アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="24cf9-105">Metadata for the device configuration user activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24cf9-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="24cf9-106">Prerequisites</span></span>
<span data-ttu-id="24cf9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24cf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24cf9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24cf9-109">Permission type</span></span>|<span data-ttu-id="24cf9-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="24cf9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24cf9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24cf9-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="24cf9-112">&nbsp;&nbsp;デバイス構成</span><span class="sxs-lookup"><span data-stu-id="24cf9-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="24cf9-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="24cf9-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="24cf9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24cf9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24cf9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24cf9-115">Not supported.</span></span>|
|<span data-ttu-id="24cf9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24cf9-116">Application</span></span>|<span data-ttu-id="24cf9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24cf9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24cf9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24cf9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="24cf9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24cf9-119">Request headers</span></span>
|<span data-ttu-id="24cf9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24cf9-120">Header</span></span>|<span data-ttu-id="24cf9-121">値</span><span class="sxs-lookup"><span data-stu-id="24cf9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24cf9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24cf9-122">Authorization</span></span>|<span data-ttu-id="24cf9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="24cf9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24cf9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="24cf9-124">Accept</span></span>|<span data-ttu-id="24cf9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24cf9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24cf9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="24cf9-126">Request body</span></span>
<span data-ttu-id="24cf9-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="24cf9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24cf9-128">応答</span><span class="sxs-lookup"><span data-stu-id="24cf9-128">Response</span></span>
<span data-ttu-id="24cf9-129">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="24cf9-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24cf9-130">例</span><span class="sxs-lookup"><span data-stu-id="24cf9-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="24cf9-131">要求</span><span class="sxs-lookup"><span data-stu-id="24cf9-131">Request</span></span>
<span data-ttu-id="24cf9-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24cf9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="24cf9-133">応答</span><span class="sxs-lookup"><span data-stu-id="24cf9-133">Response</span></span>
<span data-ttu-id="24cf9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="24cf9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








