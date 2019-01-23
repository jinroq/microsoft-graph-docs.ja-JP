---
title: getAuditActivityTypes 関数
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a5a5ee1341eea12024c9de03a111ee781ac2c184
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401769"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="bd32a-103">getAuditActivityTypes 関数</span><span class="sxs-lookup"><span data-stu-id="bd32a-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="bd32a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bd32a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd32a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd32a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd32a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bd32a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd32a-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bd32a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd32a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bd32a-108">Prerequisites</span></span>
<span data-ttu-id="bd32a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd32a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bd32a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bd32a-111">Permission type</span></span>|<span data-ttu-id="bd32a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bd32a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd32a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bd32a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd32a-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd32a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bd32a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bd32a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd32a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd32a-116">Not supported.</span></span>|
|<span data-ttu-id="bd32a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bd32a-117">Application</span></span>|<span data-ttu-id="bd32a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd32a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd32a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bd32a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="bd32a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd32a-120">Request headers</span></span>
|<span data-ttu-id="bd32a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd32a-121">Header</span></span>|<span data-ttu-id="bd32a-122">値</span><span class="sxs-lookup"><span data-stu-id="bd32a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd32a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd32a-123">Authorization</span></span>|<span data-ttu-id="bd32a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bd32a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd32a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bd32a-125">Accept</span></span>|<span data-ttu-id="bd32a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd32a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd32a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bd32a-127">Request body</span></span>
<span data-ttu-id="bd32a-128">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="bd32a-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="bd32a-129">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="bd32a-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="bd32a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd32a-130">Property</span></span>|<span data-ttu-id="bd32a-131">型</span><span class="sxs-lookup"><span data-stu-id="bd32a-131">Type</span></span>|<span data-ttu-id="bd32a-132">説明</span><span class="sxs-lookup"><span data-stu-id="bd32a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd32a-133">category</span><span class="sxs-lookup"><span data-stu-id="bd32a-133">category</span></span>|<span data-ttu-id="bd32a-134">String</span><span class="sxs-lookup"><span data-stu-id="bd32a-134">String</span></span>|<span data-ttu-id="bd32a-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bd32a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bd32a-136">応答</span><span class="sxs-lookup"><span data-stu-id="bd32a-136">Response</span></span>
<span data-ttu-id="bd32a-137">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bd32a-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd32a-138">例</span><span class="sxs-lookup"><span data-stu-id="bd32a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd32a-139">要求</span><span class="sxs-lookup"><span data-stu-id="bd32a-139">Request</span></span>
<span data-ttu-id="bd32a-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bd32a-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="bd32a-141">応答</span><span class="sxs-lookup"><span data-stu-id="bd32a-141">Response</span></span>
<span data-ttu-id="bd32a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bd32a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




