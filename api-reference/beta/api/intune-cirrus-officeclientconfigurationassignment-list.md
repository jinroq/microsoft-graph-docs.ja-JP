---
title: リスト officeClientConfigurationAssignments
description: OfficeClientConfigurationAssignment オブジェクトのプロパティとリレーションシップをリストします。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0e7698e34e2b85a45ed3e994fd955b223a86b83f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328239"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="a3286-103">リスト officeClientConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="a3286-103">List officeClientConfigurationAssignments</span></span>

> <span data-ttu-id="a3286-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3286-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3286-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3286-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3286-106">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a3286-106">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3286-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a3286-107">Prerequisites</span></span>
<span data-ttu-id="a3286-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3286-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3286-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3286-110">Permission type</span></span>|<span data-ttu-id="a3286-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3286-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3286-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3286-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3286-113">\* \* TODO: 範囲を決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="a3286-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="a3286-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3286-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3286-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3286-115">Not supported.</span></span>|
|<span data-ttu-id="a3286-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3286-116">Application</span></span>|<span data-ttu-id="a3286-117">\* \* TODO: 範囲を決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="a3286-117">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3286-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3286-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a3286-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3286-119">Request headers</span></span>
|<span data-ttu-id="a3286-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3286-120">Header</span></span>|<span data-ttu-id="a3286-121">値</span><span class="sxs-lookup"><span data-stu-id="a3286-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3286-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3286-122">Authorization</span></span>|<span data-ttu-id="a3286-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3286-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3286-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a3286-124">Accept</span></span>|<span data-ttu-id="a3286-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3286-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3286-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3286-126">Request body</span></span>
<span data-ttu-id="a3286-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a3286-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3286-128">応答</span><span class="sxs-lookup"><span data-stu-id="a3286-128">Response</span></span>
<span data-ttu-id="a3286-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a3286-129">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3286-130">例</span><span class="sxs-lookup"><span data-stu-id="a3286-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3286-131">要求</span><span class="sxs-lookup"><span data-stu-id="a3286-131">Request</span></span>
<span data-ttu-id="a3286-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a3286-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="a3286-133">応答</span><span class="sxs-lookup"><span data-stu-id="a3286-133">Response</span></span>
<span data-ttu-id="a3286-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a3286-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






