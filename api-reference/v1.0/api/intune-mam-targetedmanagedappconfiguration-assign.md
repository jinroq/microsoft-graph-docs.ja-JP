---
title: assign アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 205a79d3a765019140943a0f53dcf3462aea7c5a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261825"
---
# <a name="assign-action"></a><span data-ttu-id="df6f1-103">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="df6f1-103">assign action</span></span>

> <span data-ttu-id="df6f1-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="df6f1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df6f1-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="df6f1-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df6f1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="df6f1-106">Prerequisites</span></span>
<span data-ttu-id="df6f1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="df6f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="df6f1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="df6f1-109">Permission type</span></span>|<span data-ttu-id="df6f1-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="df6f1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df6f1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="df6f1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="df6f1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df6f1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="df6f1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="df6f1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df6f1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df6f1-114">Not supported.</span></span>|
|<span data-ttu-id="df6f1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="df6f1-115">Application</span></span>|<span data-ttu-id="df6f1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df6f1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df6f1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="df6f1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="df6f1-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df6f1-118">Request headers</span></span>
|<span data-ttu-id="df6f1-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df6f1-119">Header</span></span>|<span data-ttu-id="df6f1-120">値</span><span class="sxs-lookup"><span data-stu-id="df6f1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df6f1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="df6f1-121">Authorization</span></span>|<span data-ttu-id="df6f1-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="df6f1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df6f1-123">承諾</span><span class="sxs-lookup"><span data-stu-id="df6f1-123">Accept</span></span>|<span data-ttu-id="df6f1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="df6f1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df6f1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="df6f1-125">Request body</span></span>
<span data-ttu-id="df6f1-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="df6f1-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="df6f1-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="df6f1-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="df6f1-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df6f1-128">Property</span></span>|<span data-ttu-id="df6f1-129">型</span><span class="sxs-lookup"><span data-stu-id="df6f1-129">Type</span></span>|<span data-ttu-id="df6f1-130">説明</span><span class="sxs-lookup"><span data-stu-id="df6f1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df6f1-131">assignments</span><span class="sxs-lookup"><span data-stu-id="df6f1-131">assignments</span></span>|<span data-ttu-id="df6f1-132">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="df6f1-132">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="df6f1-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="df6f1-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="df6f1-134">応答</span><span class="sxs-lookup"><span data-stu-id="df6f1-134">Response</span></span>
<span data-ttu-id="df6f1-135">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="df6f1-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df6f1-136">例</span><span class="sxs-lookup"><span data-stu-id="df6f1-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="df6f1-137">要求</span><span class="sxs-lookup"><span data-stu-id="df6f1-137">Request</span></span>
<span data-ttu-id="df6f1-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="df6f1-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign

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

### <a name="response"></a><span data-ttu-id="df6f1-139">応答</span><span class="sxs-lookup"><span data-stu-id="df6f1-139">Response</span></span>
<span data-ttu-id="df6f1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="df6f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



