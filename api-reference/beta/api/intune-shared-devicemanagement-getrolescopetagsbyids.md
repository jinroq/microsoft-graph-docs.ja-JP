---
title: getRoleScopeTagsByIds 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 764bfd10fdfde445d38dbf5eb4f2552f02a8231f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403876"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="3d026-103">getRoleScopeTagsByIds 関数</span><span class="sxs-lookup"><span data-stu-id="3d026-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="3d026-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3d026-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3d026-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d026-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d026-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3d026-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d026-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3d026-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d026-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3d026-108">Prerequisites</span></span>
<span data-ttu-id="3d026-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d026-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d026-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3d026-111">Permission type</span></span>|<span data-ttu-id="3d026-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3d026-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d026-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3d026-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3d026-114">&nbsp;&nbsp; **ロール ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="3d026-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="3d026-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d026-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="3d026-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3d026-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d026-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d026-117">Not supported.</span></span>|
|<span data-ttu-id="3d026-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3d026-118">Application</span></span>|<span data-ttu-id="3d026-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d026-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d026-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d026-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="3d026-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d026-121">Request headers</span></span>
|<span data-ttu-id="3d026-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d026-122">Header</span></span>|<span data-ttu-id="3d026-123">値</span><span class="sxs-lookup"><span data-stu-id="3d026-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d026-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d026-124">Authorization</span></span>|<span data-ttu-id="3d026-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3d026-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d026-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3d026-126">Accept</span></span>|<span data-ttu-id="3d026-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3d026-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d026-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3d026-128">Request body</span></span>
<span data-ttu-id="3d026-129">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="3d026-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="3d026-130">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="3d026-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="3d026-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d026-131">Property</span></span>|<span data-ttu-id="3d026-132">型</span><span class="sxs-lookup"><span data-stu-id="3d026-132">Type</span></span>|<span data-ttu-id="3d026-133">説明</span><span class="sxs-lookup"><span data-stu-id="3d026-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d026-134">ids</span><span class="sxs-lookup"><span data-stu-id="3d026-134">ids</span></span>|<span data-ttu-id="3d026-135">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3d026-135">String collection</span></span>|<span data-ttu-id="3d026-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3d026-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3d026-137">応答</span><span class="sxs-lookup"><span data-stu-id="3d026-137">Response</span></span>
<span data-ttu-id="3d026-138">かどうかは成功すると、この関数を返します、`200 OK`応答コードおよび応答の本文に[roleScopeTag](../resources/intune-rbac-rolescopetag.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="3d026-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d026-139">例</span><span class="sxs-lookup"><span data-stu-id="3d026-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d026-140">要求</span><span class="sxs-lookup"><span data-stu-id="3d026-140">Request</span></span>
<span data-ttu-id="3d026-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3d026-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="3d026-142">応答</span><span class="sxs-lookup"><span data-stu-id="3d026-142">Response</span></span>
<span data-ttu-id="3d026-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3d026-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



