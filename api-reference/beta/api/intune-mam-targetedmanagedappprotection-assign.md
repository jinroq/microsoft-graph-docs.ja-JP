---
title: assign アクション
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bebc8864db76525fc34d21325ec1f67750525617
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396001"
---
# <a name="assign-action"></a><span data-ttu-id="a2479-103">assign アクション</span><span class="sxs-lookup"><span data-stu-id="a2479-103">assign action</span></span>

> <span data-ttu-id="a2479-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a2479-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a2479-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2479-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2479-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2479-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2479-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a2479-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2479-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a2479-108">Prerequisites</span></span>
<span data-ttu-id="a2479-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2479-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a2479-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2479-111">Permission type</span></span>|<span data-ttu-id="a2479-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2479-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2479-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2479-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2479-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2479-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2479-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2479-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2479-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2479-116">Not supported.</span></span>|
|<span data-ttu-id="a2479-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2479-117">Application</span></span>|<span data-ttu-id="a2479-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2479-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2479-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2479-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="a2479-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2479-120">Request headers</span></span>
|<span data-ttu-id="a2479-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2479-121">Header</span></span>|<span data-ttu-id="a2479-122">値</span><span class="sxs-lookup"><span data-stu-id="a2479-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2479-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2479-123">Authorization</span></span>|<span data-ttu-id="a2479-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a2479-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2479-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2479-125">Accept</span></span>|<span data-ttu-id="a2479-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2479-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2479-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2479-127">Request body</span></span>
<span data-ttu-id="a2479-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a2479-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a2479-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="a2479-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a2479-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2479-130">Property</span></span>|<span data-ttu-id="a2479-131">型</span><span class="sxs-lookup"><span data-stu-id="a2479-131">Type</span></span>|<span data-ttu-id="a2479-132">説明</span><span class="sxs-lookup"><span data-stu-id="a2479-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2479-133">assignments</span><span class="sxs-lookup"><span data-stu-id="a2479-133">assignments</span></span>|<span data-ttu-id="a2479-134">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2479-134">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="a2479-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a2479-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a2479-136">応答</span><span class="sxs-lookup"><span data-stu-id="a2479-136">Response</span></span>
<span data-ttu-id="a2479-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a2479-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a2479-138">例</span><span class="sxs-lookup"><span data-stu-id="a2479-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2479-139">要求</span><span class="sxs-lookup"><span data-stu-id="a2479-139">Request</span></span>
<span data-ttu-id="a2479-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a2479-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

Content-type: application/json
Content-length: 282

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a2479-141">応答</span><span class="sxs-lookup"><span data-stu-id="a2479-141">Response</span></span>
<span data-ttu-id="a2479-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a2479-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




