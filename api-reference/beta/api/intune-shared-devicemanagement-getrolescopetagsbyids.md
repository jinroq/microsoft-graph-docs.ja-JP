---
title: getRoleScopeTagsByIds 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4856b981937bbbf422d5cb8b9e30349ef492e4c1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898326"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="cd79c-103">getRoleScopeTagsByIds 関数</span><span class="sxs-lookup"><span data-stu-id="cd79c-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="cd79c-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="cd79c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cd79c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd79c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd79c-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cd79c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd79c-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cd79c-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd79c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="cd79c-108">Prerequisites</span></span>
<span data-ttu-id="cd79c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd79c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd79c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cd79c-111">Permission type</span></span>|<span data-ttu-id="cd79c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cd79c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd79c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cd79c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cd79c-114">&nbsp; &nbsp; **役割ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="cd79c-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="cd79c-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd79c-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="cd79c-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cd79c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd79c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd79c-117">Not supported.</span></span>|
|<span data-ttu-id="cd79c-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cd79c-118">Application</span></span>|<span data-ttu-id="cd79c-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd79c-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd79c-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cd79c-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="cd79c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd79c-121">Request headers</span></span>
|<span data-ttu-id="cd79c-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd79c-122">Header</span></span>|<span data-ttu-id="cd79c-123">値</span><span class="sxs-lookup"><span data-stu-id="cd79c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd79c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd79c-124">Authorization</span></span>|<span data-ttu-id="cd79c-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cd79c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd79c-126">承諾</span><span class="sxs-lookup"><span data-stu-id="cd79c-126">Accept</span></span>|<span data-ttu-id="cd79c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cd79c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd79c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="cd79c-128">Request body</span></span>
<span data-ttu-id="cd79c-129">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="cd79c-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="cd79c-130">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="cd79c-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="cd79c-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd79c-131">Property</span></span>|<span data-ttu-id="cd79c-132">型</span><span class="sxs-lookup"><span data-stu-id="cd79c-132">Type</span></span>|<span data-ttu-id="cd79c-133">説明</span><span class="sxs-lookup"><span data-stu-id="cd79c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd79c-134">ids</span><span class="sxs-lookup"><span data-stu-id="cd79c-134">ids</span></span>|<span data-ttu-id="cd79c-135">String collection</span><span class="sxs-lookup"><span data-stu-id="cd79c-135">String collection</span></span>|<span data-ttu-id="cd79c-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cd79c-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cd79c-137">応答</span><span class="sxs-lookup"><span data-stu-id="cd79c-137">Response</span></span>
<span data-ttu-id="cd79c-138">成功した場合、この関数`200 OK`は応答コードと、応答本文で[ロール copetag](../resources/intune-rbac-rolescopetag.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cd79c-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd79c-139">例</span><span class="sxs-lookup"><span data-stu-id="cd79c-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd79c-140">要求</span><span class="sxs-lookup"><span data-stu-id="cd79c-140">Request</span></span>
<span data-ttu-id="cd79c-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cd79c-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="cd79c-142">応答</span><span class="sxs-lookup"><span data-stu-id="cd79c-142">Response</span></span>
<span data-ttu-id="cd79c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cd79c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



