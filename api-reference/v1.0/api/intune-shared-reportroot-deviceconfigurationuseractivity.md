---
title: deviceConfigurationUserActivity 関数
description: デバイス構成のユーザー アクティビティ レポートのメタデータ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c83c9a6216e678d16af212f6a31648f7dea8a2b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258024"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="fa1d0-103">deviceConfigurationUserActivity 関数</span><span class="sxs-lookup"><span data-stu-id="fa1d0-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="fa1d0-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fa1d0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa1d0-105">デバイス構成のユーザー アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="fa1d0-105">Metadata for the device configuration user activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa1d0-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="fa1d0-106">Prerequisites</span></span>
<span data-ttu-id="fa1d0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa1d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa1d0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa1d0-109">Permission type</span></span>|<span data-ttu-id="fa1d0-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa1d0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa1d0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa1d0-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fa1d0-112">&nbsp;&nbsp;デバイス構成</span><span class="sxs-lookup"><span data-stu-id="fa1d0-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="fa1d0-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa1d0-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fa1d0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa1d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa1d0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa1d0-115">Not supported.</span></span>|
|<span data-ttu-id="fa1d0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa1d0-116">Application</span></span>|<span data-ttu-id="fa1d0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa1d0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa1d0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa1d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="fa1d0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa1d0-119">Request headers</span></span>
|<span data-ttu-id="fa1d0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa1d0-120">Header</span></span>|<span data-ttu-id="fa1d0-121">値</span><span class="sxs-lookup"><span data-stu-id="fa1d0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa1d0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa1d0-122">Authorization</span></span>|<span data-ttu-id="fa1d0-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fa1d0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa1d0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fa1d0-124">Accept</span></span>|<span data-ttu-id="fa1d0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa1d0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa1d0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa1d0-126">Request body</span></span>
<span data-ttu-id="fa1d0-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fa1d0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa1d0-128">応答</span><span class="sxs-lookup"><span data-stu-id="fa1d0-128">Response</span></span>
<span data-ttu-id="fa1d0-129">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="fa1d0-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa1d0-130">例</span><span class="sxs-lookup"><span data-stu-id="fa1d0-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa1d0-131">要求</span><span class="sxs-lookup"><span data-stu-id="fa1d0-131">Request</span></span>
<span data-ttu-id="fa1d0-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fa1d0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="fa1d0-133">応答</span><span class="sxs-lookup"><span data-stu-id="fa1d0-133">Response</span></span>
<span data-ttu-id="fa1d0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fa1d0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








