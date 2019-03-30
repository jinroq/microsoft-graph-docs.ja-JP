---
title: devicemanagementscriptgroupassignment の削除
description: devicemanagementscriptgroupassignment を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 296d97332b5d8627f3679a2b885244844ebb17a9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985796"
---
# <a name="delete-devicemanagementscriptgroupassignment"></a><span data-ttu-id="82d78-103">devicemanagementscriptgroupassignment の削除</span><span class="sxs-lookup"><span data-stu-id="82d78-103">Delete deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="82d78-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82d78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82d78-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="82d78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82d78-106">[devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="82d78-106">Deletes a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82d78-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="82d78-107">Prerequisites</span></span>
<span data-ttu-id="82d78-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82d78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82d78-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82d78-110">Permission type</span></span>|<span data-ttu-id="82d78-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="82d78-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82d78-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82d78-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82d78-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82d78-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="82d78-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82d78-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82d78-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82d78-115">Not supported.</span></span>|
|<span data-ttu-id="82d78-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82d78-116">Application</span></span>|<span data-ttu-id="82d78-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82d78-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82d78-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82d78-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="82d78-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82d78-119">Request headers</span></span>
|<span data-ttu-id="82d78-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82d78-120">Header</span></span>|<span data-ttu-id="82d78-121">値</span><span class="sxs-lookup"><span data-stu-id="82d78-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82d78-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82d78-122">Authorization</span></span>|<span data-ttu-id="82d78-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="82d78-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82d78-124">承諾</span><span class="sxs-lookup"><span data-stu-id="82d78-124">Accept</span></span>|<span data-ttu-id="82d78-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82d78-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82d78-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="82d78-126">Request body</span></span>
<span data-ttu-id="82d78-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="82d78-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82d78-128">応答</span><span class="sxs-lookup"><span data-stu-id="82d78-128">Response</span></span>
<span data-ttu-id="82d78-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="82d78-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="82d78-130">例</span><span class="sxs-lookup"><span data-stu-id="82d78-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="82d78-131">要求</span><span class="sxs-lookup"><span data-stu-id="82d78-131">Request</span></span>
<span data-ttu-id="82d78-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="82d78-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="82d78-133">応答</span><span class="sxs-lookup"><span data-stu-id="82d78-133">Response</span></span>
<span data-ttu-id="82d78-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="82d78-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




