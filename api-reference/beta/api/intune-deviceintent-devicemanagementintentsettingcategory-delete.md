---
title: DeviceManagementIntentSettingCategory の削除
description: DeviceManagementIntentSettingCategory を削除します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 964ee3c534abe63b3ac66a16453d07a2dcbabd1b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960175"
---
# <a name="delete-devicemanagementintentsettingcategory"></a><span data-ttu-id="dc7e2-103">DeviceManagementIntentSettingCategory の削除</span><span class="sxs-lookup"><span data-stu-id="dc7e2-103">Delete deviceManagementIntentSettingCategory</span></span>

> <span data-ttu-id="dc7e2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc7e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc7e2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dc7e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc7e2-106">[Devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="dc7e2-106">Deletes a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc7e2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="dc7e2-107">Prerequisites</span></span>
<span data-ttu-id="dc7e2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc7e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc7e2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc7e2-110">Permission type</span></span>|<span data-ttu-id="dc7e2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc7e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc7e2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dc7e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc7e2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc7e2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc7e2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc7e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc7e2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc7e2-115">Not supported.</span></span>|
|<span data-ttu-id="dc7e2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc7e2-116">Application</span></span>|<span data-ttu-id="dc7e2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc7e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc7e2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc7e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="dc7e2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc7e2-119">Request headers</span></span>
|<span data-ttu-id="dc7e2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc7e2-120">Header</span></span>|<span data-ttu-id="dc7e2-121">値</span><span class="sxs-lookup"><span data-stu-id="dc7e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc7e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc7e2-122">Authorization</span></span>|<span data-ttu-id="dc7e2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="dc7e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc7e2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="dc7e2-124">Accept</span></span>|<span data-ttu-id="dc7e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc7e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc7e2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc7e2-126">Request body</span></span>
<span data-ttu-id="dc7e2-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dc7e2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc7e2-128">応答</span><span class="sxs-lookup"><span data-stu-id="dc7e2-128">Response</span></span>
<span data-ttu-id="dc7e2-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="dc7e2-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc7e2-130">例</span><span class="sxs-lookup"><span data-stu-id="dc7e2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc7e2-131">要求</span><span class="sxs-lookup"><span data-stu-id="dc7e2-131">Request</span></span>
<span data-ttu-id="dc7e2-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dc7e2-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

### <a name="response"></a><span data-ttu-id="dc7e2-133">応答</span><span class="sxs-lookup"><span data-stu-id="dc7e2-133">Response</span></span>
<span data-ttu-id="dc7e2-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dc7e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





