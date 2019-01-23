---
title: CircularGeofenceManagementCondition を削除します。
description: CircularGeofenceManagementCondition を削除します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0ed0acd2ec46c6c1f06a2caf22b55db69cbe2088
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415916"
---
# <a name="delete-circulargeofencemanagementcondition"></a><span data-ttu-id="32c32-103">CircularGeofenceManagementCondition を削除します。</span><span class="sxs-lookup"><span data-stu-id="32c32-103">Delete circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="32c32-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="32c32-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="32c32-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32c32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32c32-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="32c32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32c32-107">の[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="32c32-107">Deletes a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32c32-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="32c32-108">Prerequisites</span></span>
<span data-ttu-id="32c32-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32c32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="32c32-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32c32-111">Permission type</span></span>|<span data-ttu-id="32c32-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="32c32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32c32-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32c32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32c32-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32c32-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32c32-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32c32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32c32-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32c32-116">Not supported.</span></span>|
|<span data-ttu-id="32c32-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32c32-117">Application</span></span>|<span data-ttu-id="32c32-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32c32-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32c32-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32c32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/managementConditions/{managementConditionId}
DELETE /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="32c32-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32c32-120">Request headers</span></span>
|<span data-ttu-id="32c32-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32c32-121">Header</span></span>|<span data-ttu-id="32c32-122">値</span><span class="sxs-lookup"><span data-stu-id="32c32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32c32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="32c32-123">Authorization</span></span>|<span data-ttu-id="32c32-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="32c32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32c32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="32c32-125">Accept</span></span>|<span data-ttu-id="32c32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32c32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32c32-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="32c32-127">Request body</span></span>
<span data-ttu-id="32c32-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="32c32-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32c32-129">応答</span><span class="sxs-lookup"><span data-stu-id="32c32-129">Response</span></span>
<span data-ttu-id="32c32-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="32c32-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="32c32-131">例</span><span class="sxs-lookup"><span data-stu-id="32c32-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="32c32-132">要求</span><span class="sxs-lookup"><span data-stu-id="32c32-132">Request</span></span>
<span data-ttu-id="32c32-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="32c32-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="32c32-134">応答</span><span class="sxs-lookup"><span data-stu-id="32c32-134">Response</span></span>
<span data-ttu-id="32c32-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="32c32-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




