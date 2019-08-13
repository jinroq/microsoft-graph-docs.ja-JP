---
title: createInstance アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf4cce6d9fd061204d56f1526e1c917c11562075
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313133"
---
# <a name="createinstance-action"></a><span data-ttu-id="a1b86-103">createInstance アクション</span><span class="sxs-lookup"><span data-stu-id="a1b86-103">createInstance action</span></span>

> <span data-ttu-id="a1b86-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1b86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1b86-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a1b86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1b86-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1b86-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1b86-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a1b86-107">Prerequisites</span></span>
<span data-ttu-id="a1b86-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1b86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1b86-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1b86-110">Permission type</span></span>|<span data-ttu-id="a1b86-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1b86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1b86-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1b86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1b86-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1b86-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1b86-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1b86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1b86-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1b86-115">Not supported.</span></span>|
|<span data-ttu-id="a1b86-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1b86-116">Application</span></span>|<span data-ttu-id="a1b86-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1b86-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1b86-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1b86-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/createInstance
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}/createInstance
```

## <a name="request-headers"></a><span data-ttu-id="a1b86-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1b86-119">Request headers</span></span>
|<span data-ttu-id="a1b86-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1b86-120">Header</span></span>|<span data-ttu-id="a1b86-121">値</span><span class="sxs-lookup"><span data-stu-id="a1b86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1b86-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1b86-122">Authorization</span></span>|<span data-ttu-id="a1b86-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a1b86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1b86-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a1b86-124">Accept</span></span>|<span data-ttu-id="a1b86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1b86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1b86-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1b86-126">Request body</span></span>
<span data-ttu-id="a1b86-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1b86-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a1b86-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="a1b86-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a1b86-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1b86-129">Property</span></span>|<span data-ttu-id="a1b86-130">型</span><span class="sxs-lookup"><span data-stu-id="a1b86-130">Type</span></span>|<span data-ttu-id="a1b86-131">説明</span><span class="sxs-lookup"><span data-stu-id="a1b86-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1b86-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a1b86-132">displayName</span></span>|<span data-ttu-id="a1b86-133">String</span><span class="sxs-lookup"><span data-stu-id="a1b86-133">String</span></span>|<span data-ttu-id="a1b86-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1b86-134">Not yet documented</span></span>|
|<span data-ttu-id="a1b86-135">description</span><span class="sxs-lookup"><span data-stu-id="a1b86-135">description</span></span>|<span data-ttu-id="a1b86-136">String</span><span class="sxs-lookup"><span data-stu-id="a1b86-136">String</span></span>|<span data-ttu-id="a1b86-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1b86-137">Not yet documented</span></span>|
|<span data-ttu-id="a1b86-138">settingsDelta</span><span class="sxs-lookup"><span data-stu-id="a1b86-138">settingsDelta</span></span>|<span data-ttu-id="a1b86-139">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a1b86-139">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="a1b86-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1b86-140">Not yet documented</span></span>|
|<span data-ttu-id="a1b86-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a1b86-141">roleScopeTagIds</span></span>|<span data-ttu-id="a1b86-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a1b86-142">String collection</span></span>|<span data-ttu-id="a1b86-143">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1b86-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a1b86-144">応答</span><span class="sxs-lookup"><span data-stu-id="a1b86-144">Response</span></span>
<span data-ttu-id="a1b86-145">成功した場合、このアクション`200 OK`は応答コードと、応答本文で[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="a1b86-145">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1b86-146">例</span><span class="sxs-lookup"><span data-stu-id="a1b86-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1b86-147">要求</span><span class="sxs-lookup"><span data-stu-id="a1b86-147">Request</span></span>
<span data-ttu-id="a1b86-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a1b86-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/createInstance

Content-type: application/json
Content-length: 398

{
  "displayName": "Display Name value",
  "description": "Description value",
  "settingsDelta": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
      "id": "d68168e1-68e1-d681-e168-81d6e16881d6",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="a1b86-149">応答</span><span class="sxs-lookup"><span data-stu-id="a1b86-149">Response</span></span>
<span data-ttu-id="a1b86-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a1b86-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 418

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntent",
    "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
    "displayName": "Display Name value",
    "description": "Description value",
    "isAssigned": true,
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "templateId": "Template Id value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```






