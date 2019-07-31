---
title: setDefaultProfile アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cea1ab69347cb0e6c60769b9d8cb8254b2b8ebec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35980996"
---
# <a name="setdefaultprofile-action"></a><span data-ttu-id="ebe94-103">setDefaultProfile アクション</span><span class="sxs-lookup"><span data-stu-id="ebe94-103">setDefaultProfile action</span></span>

> <span data-ttu-id="ebe94-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebe94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebe94-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ebe94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebe94-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ebe94-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebe94-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ebe94-107">Prerequisites</span></span>
<span data-ttu-id="ebe94-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebe94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebe94-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ebe94-110">Permission type</span></span>|<span data-ttu-id="ebe94-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ebe94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebe94-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ebe94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebe94-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebe94-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ebe94-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ebe94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebe94-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebe94-115">Not supported.</span></span>|
|<span data-ttu-id="ebe94-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ebe94-116">Application</span></span>|<span data-ttu-id="ebe94-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebe94-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebe94-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ebe94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/setDefaultProfile
```

## <a name="request-headers"></a><span data-ttu-id="ebe94-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebe94-119">Request headers</span></span>
|<span data-ttu-id="ebe94-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebe94-120">Header</span></span>|<span data-ttu-id="ebe94-121">値</span><span class="sxs-lookup"><span data-stu-id="ebe94-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebe94-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebe94-122">Authorization</span></span>|<span data-ttu-id="ebe94-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ebe94-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebe94-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ebe94-124">Accept</span></span>|<span data-ttu-id="ebe94-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ebe94-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebe94-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ebe94-126">Request body</span></span>
<span data-ttu-id="ebe94-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ebe94-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebe94-128">応答</span><span class="sxs-lookup"><span data-stu-id="ebe94-128">Response</span></span>
<span data-ttu-id="ebe94-129">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ebe94-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ebe94-130">例</span><span class="sxs-lookup"><span data-stu-id="ebe94-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebe94-131">要求</span><span class="sxs-lookup"><span data-stu-id="ebe94-131">Request</span></span>
<span data-ttu-id="ebe94-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ebe94-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/setDefaultProfile
```

### <a name="response"></a><span data-ttu-id="ebe94-133">応答</span><span class="sxs-lookup"><span data-stu-id="ebe94-133">Response</span></span>
<span data-ttu-id="ebe94-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ebe94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





