---
title: microsoft Intune での会社の使用条件-microsoft Graph API
description: テナント組織の使用条件を定義する Intune エンドポイント (REST) の Microsoft Graph API を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 1277a6893ddd306b7050fafc70b815217d376b14
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172283"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a>Microsoft Intune の会社の使用条件

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

Intune の使用条件をユーザー グループに展開して、登録、作業リソースへのアクセス、ポータル サイト アプリがデバイスやユーザーにどのように影響するかを説明することができます。 ポータル サイトを使用して自分の仕事に登録してアクセスするには、ユーザーはまず使用条件に同意する必要があります。

さまざまな使用条件を含む複数のポリシーを作成して展開することができます。 同じ使用条件のバージョンを異なる言語で作成し、それぞれ適切なグループに展開することもできます。

次の Graph リソースを使用して、Intune での会社の使用条件を管理できます。

- [使用条件](intune-companyterms-termsandconditions.md)
- [使用条件の承認状態](intune-companyterms-termsandconditionsacceptancestatus.md)
- [使用条件の割り当て](intune-companyterms-termsandconditionsassignment.md)
- [条項および条件のグループの割り当て](intune-companyterms-termsandconditionsgroupassignment.md)
