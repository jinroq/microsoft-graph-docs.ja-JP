---
title: assign アクション
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3ec08c34c6580643f47b4e09eb191031f6b29ef3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428907"
---
# <a name="assign-action"></a><span data-ttu-id="66efd-103">assign アクション</span><span class="sxs-lookup"><span data-stu-id="66efd-103">assign action</span></span>

> <span data-ttu-id="66efd-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="66efd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="66efd-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66efd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66efd-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="66efd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66efd-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="66efd-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66efd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="66efd-108">Prerequisites</span></span>
<span data-ttu-id="66efd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66efd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="66efd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66efd-111">Permission type</span></span>|<span data-ttu-id="66efd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="66efd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66efd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66efd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66efd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66efd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66efd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66efd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66efd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66efd-116">Not supported.</span></span>|
|<span data-ttu-id="66efd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66efd-117">Application</span></span>|<span data-ttu-id="66efd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66efd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66efd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66efd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="66efd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66efd-120">Request headers</span></span>
|<span data-ttu-id="66efd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66efd-121">Header</span></span>|<span data-ttu-id="66efd-122">値</span><span class="sxs-lookup"><span data-stu-id="66efd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66efd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66efd-123">Authorization</span></span>|<span data-ttu-id="66efd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="66efd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66efd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="66efd-125">Accept</span></span>|<span data-ttu-id="66efd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66efd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66efd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="66efd-127">Request body</span></span>
<span data-ttu-id="66efd-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="66efd-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="66efd-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="66efd-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="66efd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66efd-130">Property</span></span>|<span data-ttu-id="66efd-131">型</span><span class="sxs-lookup"><span data-stu-id="66efd-131">Type</span></span>|<span data-ttu-id="66efd-132">説明</span><span class="sxs-lookup"><span data-stu-id="66efd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66efd-133">assignments</span><span class="sxs-lookup"><span data-stu-id="66efd-133">assignments</span></span>|<span data-ttu-id="66efd-134">[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="66efd-134">[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) collection</span></span>|<span data-ttu-id="66efd-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="66efd-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="66efd-136">応答</span><span class="sxs-lookup"><span data-stu-id="66efd-136">Response</span></span>
<span data-ttu-id="66efd-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="66efd-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="66efd-138">例</span><span class="sxs-lookup"><span data-stu-id="66efd-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="66efd-139">要求</span><span class="sxs-lookup"><span data-stu-id="66efd-139">Request</span></span>
<span data-ttu-id="66efd-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="66efd-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign

Content-type: application/json
Content-length: 279

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
      "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="66efd-141">応答</span><span class="sxs-lookup"><span data-stu-id="66efd-141">Response</span></span>
<span data-ttu-id="66efd-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="66efd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




