---
title: assign アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef23b1e9c5f8a67975d8b7eb8dd9e609fb882080
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256498"
---
# <a name="assign-action"></a><span data-ttu-id="13650-103">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="13650-103">assign action</span></span>

> <span data-ttu-id="13650-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="13650-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13650-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="13650-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13650-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="13650-106">Prerequisites</span></span>
<span data-ttu-id="13650-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13650-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="13650-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13650-109">Permission type</span></span>|<span data-ttu-id="13650-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="13650-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13650-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13650-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13650-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13650-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="13650-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13650-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13650-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13650-114">Not supported.</span></span>|
|<span data-ttu-id="13650-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13650-115">Application</span></span>|<span data-ttu-id="13650-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13650-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13650-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13650-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="13650-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13650-118">Request headers</span></span>
|<span data-ttu-id="13650-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13650-119">Header</span></span>|<span data-ttu-id="13650-120">値</span><span class="sxs-lookup"><span data-stu-id="13650-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13650-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="13650-121">Authorization</span></span>|<span data-ttu-id="13650-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="13650-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13650-123">承諾</span><span class="sxs-lookup"><span data-stu-id="13650-123">Accept</span></span>|<span data-ttu-id="13650-124">application/json</span><span class="sxs-lookup"><span data-stu-id="13650-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13650-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="13650-125">Request body</span></span>
<span data-ttu-id="13650-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="13650-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="13650-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="13650-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="13650-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13650-128">Property</span></span>|<span data-ttu-id="13650-129">型</span><span class="sxs-lookup"><span data-stu-id="13650-129">Type</span></span>|<span data-ttu-id="13650-130">説明</span><span class="sxs-lookup"><span data-stu-id="13650-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13650-131">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="13650-131">mobileAppAssignments</span></span>|<span data-ttu-id="13650-132">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="13650-132">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="13650-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="13650-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="13650-134">応答</span><span class="sxs-lookup"><span data-stu-id="13650-134">Response</span></span>
<span data-ttu-id="13650-135">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="13650-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="13650-136">例</span><span class="sxs-lookup"><span data-stu-id="13650-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="13650-137">要求</span><span class="sxs-lookup"><span data-stu-id="13650-137">Request</span></span>
<span data-ttu-id="13650-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="13650-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assign

Content-type: application/json
Content-length: 406

{
  "mobileAppAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="13650-139">応答</span><span class="sxs-lookup"><span data-stu-id="13650-139">Response</span></span>
<span data-ttu-id="13650-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="13650-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



