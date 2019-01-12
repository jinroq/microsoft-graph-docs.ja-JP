---
title: getRoleScopeTagsByResource 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5ae72cf87d75d7cfd7c1652f5979932ae71e29f8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968380"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="e0b35-103">getRoleScopeTagsByResource 関数</span><span class="sxs-lookup"><span data-stu-id="e0b35-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="e0b35-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e0b35-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0b35-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0b35-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0b35-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0b35-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0b35-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e0b35-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0b35-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e0b35-108">Prerequisites</span></span>
<span data-ttu-id="e0b35-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0b35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0b35-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e0b35-111">Permission type</span></span>|<span data-ttu-id="e0b35-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e0b35-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0b35-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e0b35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0b35-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0b35-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="e0b35-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e0b35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0b35-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0b35-116">Not supported.</span></span>|
|<span data-ttu-id="e0b35-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e0b35-117">Application</span></span>|<span data-ttu-id="e0b35-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0b35-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0b35-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e0b35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="e0b35-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0b35-120">Request headers</span></span>
|<span data-ttu-id="e0b35-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0b35-121">Header</span></span>|<span data-ttu-id="e0b35-122">値</span><span class="sxs-lookup"><span data-stu-id="e0b35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0b35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0b35-123">Authorization</span></span>|<span data-ttu-id="e0b35-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e0b35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0b35-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0b35-125">Accept</span></span>|<span data-ttu-id="e0b35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0b35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0b35-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e0b35-127">Request body</span></span>
<span data-ttu-id="e0b35-128">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e0b35-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e0b35-129">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="e0b35-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e0b35-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0b35-130">Property</span></span>|<span data-ttu-id="e0b35-131">種類</span><span class="sxs-lookup"><span data-stu-id="e0b35-131">Type</span></span>|<span data-ttu-id="e0b35-132">説明</span><span class="sxs-lookup"><span data-stu-id="e0b35-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0b35-133">リソース</span><span class="sxs-lookup"><span data-stu-id="e0b35-133">resource</span></span>|<span data-ttu-id="e0b35-134">String</span><span class="sxs-lookup"><span data-stu-id="e0b35-134">String</span></span>|<span data-ttu-id="e0b35-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e0b35-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e0b35-136">応答</span><span class="sxs-lookup"><span data-stu-id="e0b35-136">Response</span></span>
<span data-ttu-id="e0b35-137">かどうかは成功すると、この関数を返します、`200 OK`応答コードおよび応答の本文に[roleScopeTag](../resources/intune-rbac-rolescopetag.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="e0b35-137">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0b35-138">例</span><span class="sxs-lookup"><span data-stu-id="e0b35-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0b35-139">要求</span><span class="sxs-lookup"><span data-stu-id="e0b35-139">Request</span></span>
<span data-ttu-id="e0b35-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e0b35-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e0b35-141">応答</span><span class="sxs-lookup"><span data-stu-id="e0b35-141">Response</span></span>
<span data-ttu-id="e0b35-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e0b35-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 231

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```





