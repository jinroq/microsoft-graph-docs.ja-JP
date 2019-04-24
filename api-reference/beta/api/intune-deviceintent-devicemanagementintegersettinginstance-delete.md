---
title: devicemanagement整数 settinginstance の削除
description: devicemanagement整数の settinginstance を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce9bfd2eb8c7cec359964184ca2ef8625246ed95
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32509423"
---
# <a name="delete-devicemanagementintegersettinginstance"></a><span data-ttu-id="a1436-103">devicemanagement整数 settinginstance の削除</span><span class="sxs-lookup"><span data-stu-id="a1436-103">Delete deviceManagementIntegerSettingInstance</span></span>

> <span data-ttu-id="a1436-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1436-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1436-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a1436-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1436-106">[devicemanagement整数の settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="a1436-106">Deletes a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1436-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a1436-107">Prerequisites</span></span>
<span data-ttu-id="a1436-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1436-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1436-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1436-110">Permission type</span></span>|<span data-ttu-id="a1436-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1436-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1436-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1436-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1436-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1436-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1436-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1436-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1436-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1436-115">Not supported.</span></span>|
|<span data-ttu-id="a1436-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1436-116">Application</span></span>|<span data-ttu-id="a1436-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1436-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1436-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1436-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
DELETE /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
DELETE /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
DELETE /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="request-headers"></a><span data-ttu-id="a1436-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1436-119">Request headers</span></span>
|<span data-ttu-id="a1436-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1436-120">Header</span></span>|<span data-ttu-id="a1436-121">値</span><span class="sxs-lookup"><span data-stu-id="a1436-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1436-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1436-122">Authorization</span></span>|<span data-ttu-id="a1436-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a1436-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1436-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a1436-124">Accept</span></span>|<span data-ttu-id="a1436-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1436-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1436-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1436-126">Request body</span></span>
<span data-ttu-id="a1436-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a1436-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1436-128">応答</span><span class="sxs-lookup"><span data-stu-id="a1436-128">Response</span></span>
<span data-ttu-id="a1436-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a1436-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a1436-130">例</span><span class="sxs-lookup"><span data-stu-id="a1436-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1436-131">要求</span><span class="sxs-lookup"><span data-stu-id="a1436-131">Request</span></span>
<span data-ttu-id="a1436-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a1436-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="a1436-133">応答</span><span class="sxs-lookup"><span data-stu-id="a1436-133">Response</span></span>
<span data-ttu-id="a1436-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a1436-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





