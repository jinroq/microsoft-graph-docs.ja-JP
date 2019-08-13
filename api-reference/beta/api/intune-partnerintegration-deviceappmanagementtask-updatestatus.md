---
title: updateStatus アクション
description: タスクの状態を設定し、メモを添付します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b504a3aa862db913c502276b01f264be86c81ce2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36351666"
---
# <a name="updatestatus-action"></a><span data-ttu-id="82034-103">updateStatus アクション</span><span class="sxs-lookup"><span data-stu-id="82034-103">updateStatus action</span></span>

> <span data-ttu-id="82034-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82034-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82034-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="82034-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82034-106">タスクの状態を設定し、メモを添付します。</span><span class="sxs-lookup"><span data-stu-id="82034-106">Set the task's status and attach a note.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82034-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="82034-107">Prerequisites</span></span>
<span data-ttu-id="82034-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82034-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82034-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82034-110">Permission type</span></span>|<span data-ttu-id="82034-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="82034-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82034-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82034-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82034-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82034-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="82034-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82034-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82034-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82034-115">Not supported.</span></span>|
|<span data-ttu-id="82034-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82034-116">Application</span></span>|<span data-ttu-id="82034-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82034-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82034-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82034-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus
```

## <a name="request-headers"></a><span data-ttu-id="82034-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82034-119">Request headers</span></span>
|<span data-ttu-id="82034-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82034-120">Header</span></span>|<span data-ttu-id="82034-121">値</span><span class="sxs-lookup"><span data-stu-id="82034-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82034-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82034-122">Authorization</span></span>|<span data-ttu-id="82034-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="82034-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82034-124">承諾</span><span class="sxs-lookup"><span data-stu-id="82034-124">Accept</span></span>|<span data-ttu-id="82034-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82034-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82034-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="82034-126">Request body</span></span>
<span data-ttu-id="82034-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="82034-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="82034-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="82034-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="82034-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82034-129">Property</span></span>|<span data-ttu-id="82034-130">型</span><span class="sxs-lookup"><span data-stu-id="82034-130">Type</span></span>|<span data-ttu-id="82034-131">説明</span><span class="sxs-lookup"><span data-stu-id="82034-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82034-132">status</span><span class="sxs-lookup"><span data-stu-id="82034-132">status</span></span>|[<span data-ttu-id="82034-133">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="82034-133">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="82034-134">状態</span><span class="sxs-lookup"><span data-stu-id="82034-134">The status</span></span>|
|<span data-ttu-id="82034-135">こと</span><span class="sxs-lookup"><span data-stu-id="82034-135">note</span></span>|<span data-ttu-id="82034-136">String</span><span class="sxs-lookup"><span data-stu-id="82034-136">String</span></span>|<span data-ttu-id="82034-137">メモ</span><span class="sxs-lookup"><span data-stu-id="82034-137">The note</span></span>|



## <a name="response"></a><span data-ttu-id="82034-138">応答</span><span class="sxs-lookup"><span data-stu-id="82034-138">Response</span></span>
<span data-ttu-id="82034-139">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="82034-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="82034-140">例</span><span class="sxs-lookup"><span data-stu-id="82034-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="82034-141">要求</span><span class="sxs-lookup"><span data-stu-id="82034-141">Request</span></span>
<span data-ttu-id="82034-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="82034-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus

Content-type: application/json
Content-length: 52

{
  "status": "pending",
  "note": "Note value"
}
```

### <a name="response"></a><span data-ttu-id="82034-143">応答</span><span class="sxs-lookup"><span data-stu-id="82034-143">Response</span></span>
<span data-ttu-id="82034-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="82034-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






