---
title: intuneBrandingProfile の削除
description: intuneBrandingProfile を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b5aeea498a229280c348ff0a94045b0bc35b00d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541795"
---
# <a name="delete-intunebrandingprofile"></a><span data-ttu-id="45aff-103">intuneBrandingProfile の削除</span><span class="sxs-lookup"><span data-stu-id="45aff-103">Delete intuneBrandingProfile</span></span>

> <span data-ttu-id="45aff-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45aff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45aff-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="45aff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45aff-106">[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="45aff-106">Deletes a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45aff-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="45aff-107">Prerequisites</span></span>
<span data-ttu-id="45aff-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45aff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45aff-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="45aff-110">Permission type</span></span>|<span data-ttu-id="45aff-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="45aff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45aff-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="45aff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45aff-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45aff-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45aff-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="45aff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45aff-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45aff-115">Not supported.</span></span>|
|<span data-ttu-id="45aff-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="45aff-116">Application</span></span>|<span data-ttu-id="45aff-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45aff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45aff-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="45aff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="45aff-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45aff-119">Request headers</span></span>
|<span data-ttu-id="45aff-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45aff-120">Header</span></span>|<span data-ttu-id="45aff-121">値</span><span class="sxs-lookup"><span data-stu-id="45aff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45aff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="45aff-122">Authorization</span></span>|<span data-ttu-id="45aff-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="45aff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45aff-124">承諾</span><span class="sxs-lookup"><span data-stu-id="45aff-124">Accept</span></span>|<span data-ttu-id="45aff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45aff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45aff-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="45aff-126">Request body</span></span>
<span data-ttu-id="45aff-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="45aff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45aff-128">応答</span><span class="sxs-lookup"><span data-stu-id="45aff-128">Response</span></span>
<span data-ttu-id="45aff-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="45aff-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="45aff-130">例</span><span class="sxs-lookup"><span data-stu-id="45aff-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="45aff-131">要求</span><span class="sxs-lookup"><span data-stu-id="45aff-131">Request</span></span>
<span data-ttu-id="45aff-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="45aff-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="45aff-133">応答</span><span class="sxs-lookup"><span data-stu-id="45aff-133">Response</span></span>
<span data-ttu-id="45aff-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="45aff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





