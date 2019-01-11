---
title: getRoleScopeTagsByIds 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dd5389c4cece513bfaea434192fd612dd60bc239
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868335"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="7aae0-103">getRoleScopeTagsByIds 関数</span><span class="sxs-lookup"><span data-stu-id="7aae0-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="7aae0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7aae0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7aae0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7aae0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7aae0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7aae0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7aae0-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7aae0-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7aae0-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7aae0-108">Prerequisites</span></span>
<span data-ttu-id="7aae0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7aae0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aae0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7aae0-111">Permission type</span></span>|<span data-ttu-id="7aae0-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7aae0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7aae0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7aae0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7aae0-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aae0-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="7aae0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7aae0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7aae0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7aae0-116">Not supported.</span></span>|
|<span data-ttu-id="7aae0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7aae0-117">Application</span></span>|<span data-ttu-id="7aae0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7aae0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7aae0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7aae0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="7aae0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7aae0-120">Request headers</span></span>
|<span data-ttu-id="7aae0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7aae0-121">Header</span></span>|<span data-ttu-id="7aae0-122">値</span><span class="sxs-lookup"><span data-stu-id="7aae0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7aae0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aae0-123">Authorization</span></span>|<span data-ttu-id="7aae0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7aae0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7aae0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7aae0-125">Accept</span></span>|<span data-ttu-id="7aae0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7aae0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7aae0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7aae0-127">Request body</span></span>
<span data-ttu-id="7aae0-128">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7aae0-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7aae0-129">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="7aae0-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7aae0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7aae0-130">Property</span></span>|<span data-ttu-id="7aae0-131">種類</span><span class="sxs-lookup"><span data-stu-id="7aae0-131">Type</span></span>|<span data-ttu-id="7aae0-132">説明</span><span class="sxs-lookup"><span data-stu-id="7aae0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7aae0-133">ids</span><span class="sxs-lookup"><span data-stu-id="7aae0-133">ids</span></span>|<span data-ttu-id="7aae0-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7aae0-134">String collection</span></span>|<span data-ttu-id="7aae0-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7aae0-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7aae0-136">応答</span><span class="sxs-lookup"><span data-stu-id="7aae0-136">Response</span></span>
<span data-ttu-id="7aae0-137">かどうかは成功すると、この関数を返します、`200 OK`応答コードおよび応答の本文に[roleScopeTag](../resources/intune-rbac-rolescopetag.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="7aae0-137">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aae0-138">例</span><span class="sxs-lookup"><span data-stu-id="7aae0-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="7aae0-139">要求</span><span class="sxs-lookup"><span data-stu-id="7aae0-139">Request</span></span>
<span data-ttu-id="7aae0-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7aae0-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="7aae0-141">応答</span><span class="sxs-lookup"><span data-stu-id="7aae0-141">Response</span></span>
<span data-ttu-id="7aae0-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7aae0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





