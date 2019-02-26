---
title: getManagementConditionStatementsForPlatform 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b0b3131df9b7edd1652885fe8415f3862eaf6ef
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149043"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="ca34d-103">getManagementConditionStatementsForPlatform 関数</span><span class="sxs-lookup"><span data-stu-id="ca34d-103">getManagementConditionStatementsForPlatform function</span></span>

> <span data-ttu-id="ca34d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca34d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca34d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ca34d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca34d-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ca34d-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca34d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ca34d-107">Prerequisites</span></span>
<span data-ttu-id="ca34d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca34d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ca34d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ca34d-110">Permission type</span></span>|<span data-ttu-id="ca34d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ca34d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca34d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ca34d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca34d-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca34d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ca34d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca34d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca34d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca34d-115">Not supported.</span></span>|
|<span data-ttu-id="ca34d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ca34d-116">Application</span></span>|<span data-ttu-id="ca34d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca34d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca34d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ca34d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="ca34d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca34d-119">Request headers</span></span>
|<span data-ttu-id="ca34d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca34d-120">Header</span></span>|<span data-ttu-id="ca34d-121">値</span><span class="sxs-lookup"><span data-stu-id="ca34d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca34d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca34d-122">Authorization</span></span>|<span data-ttu-id="ca34d-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ca34d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca34d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ca34d-124">Accept</span></span>|<span data-ttu-id="ca34d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca34d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca34d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ca34d-126">Request body</span></span>
<span data-ttu-id="ca34d-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ca34d-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ca34d-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="ca34d-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ca34d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca34d-129">Property</span></span>|<span data-ttu-id="ca34d-130">型</span><span class="sxs-lookup"><span data-stu-id="ca34d-130">Type</span></span>|<span data-ttu-id="ca34d-131">説明</span><span class="sxs-lookup"><span data-stu-id="ca34d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca34d-132">platform</span><span class="sxs-lookup"><span data-stu-id="ca34d-132">platform</span></span>|[<span data-ttu-id="ca34d-133">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="ca34d-133">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="ca34d-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ca34d-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ca34d-135">応答</span><span class="sxs-lookup"><span data-stu-id="ca34d-135">Response</span></span>
<span data-ttu-id="ca34d-136">成功した場合、この関数`200 OK`は応答コードと、応答本文で[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ca34d-136">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca34d-137">例</span><span class="sxs-lookup"><span data-stu-id="ca34d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca34d-138">要求</span><span class="sxs-lookup"><span data-stu-id="ca34d-138">Request</span></span>
<span data-ttu-id="ca34d-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ca34d-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ca34d-140">応答</span><span class="sxs-lookup"><span data-stu-id="ca34d-140">Response</span></span>
<span data-ttu-id="ca34d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ca34d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementConditionStatement",
      "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "expression": {
        "@odata.type": "microsoft.graph.managementConditionExpression"
      },
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```




