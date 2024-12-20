- DONE finish the transfer page, and the transactions page. 
- DONE Transfers endpint shows all transfers for all users instead of related users
- DONE design the dashboard
- DONE calculate all wallets balances
- DONE chart  recent activity chart
- DONE do a logout endpoint
- DONE Do I need a refresh token machinsem? 


## try the real-time updates later on

import { io } from 'socket.io-client';

const socket = io('http://localhost:3000'); // Adjust the URL as needed

socket.on('connect', () => {
console.log('Connected to WebSocket server');
});

socket.on('balanceUpdate', (data) => {
console.log(`Wallet ${data.walletId} balance updated: ${data.newBalance}`);
});
