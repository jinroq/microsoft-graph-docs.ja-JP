---
title: getRoleScopeTagsByResource 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 736c1d8c874d0eb5ae2ce42ac9b9f17a98554879
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890560"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="d5004-103">getRoleScopeTagsByResource 関数</span><span class="sxs-lookup"><span data-stu-id="d5004-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="d5004-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d5004-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5004-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5004-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5004-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5004-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5004-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d5004-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5004-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d5004-108">Prerequisites</span></span>
<span data-ttu-id="d5004-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5004-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5004-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5004-111">Permission type</span></span>|<span data-ttu-id="d5004-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5004-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5004-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5004-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d5004-114">&nbsp;&nbsp; **ロール ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="d5004-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="d5004-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5004-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="d5004-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5004-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5004-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5004-117">Not supported.</span></span>|
|<span data-ttu-id="d5004-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5004-118">Application</span></span>|<span data-ttu-id="d5004-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5004-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5004-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5004-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="d5004-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5004-121">Request headers</span></span>
|<span data-ttu-id="d5004-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5004-122">Header</span></span>|<span data-ttu-id="d5004-123">値</span><span class="sxs-lookup"><span data-stu-id="d5004-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5004-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5004-124">Authorization</span></span>|<span data-ttu-id="d5004-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d5004-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5004-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d5004-126">Accept</span></span>|<span data-ttu-id="d5004-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d5004-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5004-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5004-128">Request body</span></span>
<span data-ttu-id="d5004-129">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d5004-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d5004-130">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="d5004-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d5004-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5004-131">Property</span></span>|<span data-ttu-id="d5004-132">種類</span><span class="sxs-lookup"><span data-stu-id="d5004-132">Type</span></span>|<span data-ttu-id="d5004-133">説明</span><span class="sxs-lookup"><span data-stu-id="d5004-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5004-134">リソース</span><span class="sxs-lookup"><span data-stu-id="d5004-134">resource</span></span>|<span data-ttu-id="d5004-135">String</span><span class="sxs-lookup"><span data-stu-id="d5004-135">String</span></span>|<span data-ttu-id="d5004-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d5004-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d5004-137">応答</span><span class="sxs-lookup"><span data-stu-id="d5004-137">Response</span></span>
<span data-ttu-id="d5004-138">かどうかは成功すると、この関数を返します、`200 OK`応答コードおよび応答の本文に[roleScopeTag](../resources/intune-rbac-rolescopetag.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="d5004-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5004-139">例</span><span class="sxs-lookup"><span data-stu-id="d5004-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5004-140">要求</span><span class="sxs-lookup"><span data-stu-id="d5004-140">Request</span></span>
<span data-ttu-id="d5004-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d5004-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d5004-142">応答</span><span class="sxs-lookup"><span data-stu-id="d5004-142">Response</span></span>
<span data-ttu-id="d5004-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d5004-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



