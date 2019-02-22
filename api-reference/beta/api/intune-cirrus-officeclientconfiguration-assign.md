---
title: assign アクション
description: ポリシーの対象グループをすべて置換します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b6dfde86fe1163ea7cb9f86720a979c79e99671c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145662"
---
# <a name="assign-action"></a><span data-ttu-id="27bc9-103">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="27bc9-103">assign action</span></span>

> <span data-ttu-id="27bc9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27bc9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27bc9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="27bc9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27bc9-106">ポリシーの対象グループをすべて置換します。</span><span class="sxs-lookup"><span data-stu-id="27bc9-106">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27bc9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="27bc9-107">Prerequisites</span></span>
<span data-ttu-id="27bc9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27bc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27bc9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27bc9-110">Permission type</span></span>|<span data-ttu-id="27bc9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="27bc9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27bc9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="27bc9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27bc9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27bc9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27bc9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27bc9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27bc9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27bc9-115">Not supported.</span></span>|
|<span data-ttu-id="27bc9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27bc9-116">Application</span></span>|<span data-ttu-id="27bc9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27bc9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27bc9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27bc9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="27bc9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27bc9-119">Request headers</span></span>
|<span data-ttu-id="27bc9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27bc9-120">Header</span></span>|<span data-ttu-id="27bc9-121">値</span><span class="sxs-lookup"><span data-stu-id="27bc9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27bc9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="27bc9-122">Authorization</span></span>|<span data-ttu-id="27bc9-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="27bc9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27bc9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="27bc9-124">Accept</span></span>|<span data-ttu-id="27bc9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27bc9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27bc9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="27bc9-126">Request body</span></span>
<span data-ttu-id="27bc9-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="27bc9-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="27bc9-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="27bc9-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="27bc9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27bc9-129">Property</span></span>|<span data-ttu-id="27bc9-130">型</span><span class="sxs-lookup"><span data-stu-id="27bc9-130">Type</span></span>|<span data-ttu-id="27bc9-131">説明</span><span class="sxs-lookup"><span data-stu-id="27bc9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27bc9-132">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="27bc9-132">officeConfigurationAssignments</span></span>|<span data-ttu-id="27bc9-133">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="27bc9-133">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="27bc9-134">office の構成割り当ての一覧</span><span class="sxs-lookup"><span data-stu-id="27bc9-134">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="27bc9-135">応答</span><span class="sxs-lookup"><span data-stu-id="27bc9-135">Response</span></span>
<span data-ttu-id="27bc9-136">成功した場合、このアクション`200 OK`は応答コードと、応答本文で[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="27bc9-136">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27bc9-137">例</span><span class="sxs-lookup"><span data-stu-id="27bc9-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="27bc9-138">要求</span><span class="sxs-lookup"><span data-stu-id="27bc9-138">Request</span></span>
<span data-ttu-id="27bc9-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="27bc9-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign

Content-type: application/json
Content-length: 299

{
  "officeConfigurationAssignments": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="27bc9-140">応答</span><span class="sxs-lookup"><span data-stu-id="27bc9-140">Response</span></span>
<span data-ttu-id="27bc9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="27bc9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```



